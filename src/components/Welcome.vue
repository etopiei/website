<template>
  <v-container>
    <v-layout
      text-xs-center
      wrap
    >
      <v-flex xs12>
        <v-img
          :src="require('../assets/comp_website.jpeg')"
          contain
          height="200"
        ></v-img>
      </v-flex>
      <v-flex mb-4>
        <h1 class="display-2 font-weight-bold mb-3">
          <br> Hi! I'm Lachlan. <br>
          Welcome to my website.
        </h1>
        <p class="subheading font-weight-regular">
          📖 Monash University - Computer Science Student<br>
          💰 National Australia Bank - Intern Software Engineer<br>
          💻 AI Media - Software Developer<br>
        </p>
        <h2>GitHub Latest Projects</h2>
        <p v-if="loading">
        ... Loading Recent Public Projects ...
        </p>
        <div class="github_projects">
          <v-flex class="project" v-for="(item, index) in projectData" :key="index" xs6>
            <v-card color="rgb(145, 212, 255)" height="180px" class="white--text">
              <v-card-title class="black--text" primary-title>
                <div>
                  <div class="headline">{{item.name}}</div>
                  <span>{{item.description}}</span>
                </div>
              </v-card-title>
              <v-card-actions>
                <v-btn class="black--text" flat dark>View</v-btn>
              </v-card-actions>
            </v-card>
          </v-flex>
        </div>
      </v-flex>
      <v-flex mb-4>
        <h2> More About Me </h2>
        <p>I am passionate about open source, privacy and about learning as much as I can.
          When I'm not working on software I might be found playing guitar, running, playing chess or writing my blog.
        </p>
      </v-flex>
      <v-flex mb-4>
        <h2> Contact Me </h2>
        <span>Twitter: @etopiei</span><br>
        <span>Email: me.etopiei@gmail.com</span>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    mounted() {
      const repos = [];
      fetch('https://api.github.com/users/etopiei/repos').then((res) => res.json()).then((serverData) => {
        // sort by latest update and remove projects that are forks
        const sortedData = serverData.sort((a, b) => b.updated_at > a.updated_at).filter((item) => !item.fork);
        sortedData.forEach((repo) => {
          if (repos.length < 4) {
            repos.push({name: repo.name, description: repo.description, url: repo.html_url, language: repo.language});
          }
        });
        this.loading = false;
        this.projectData = repos;
      });
    },
    data: () => ({
      loading: true,
      projectData: null,
    }),
  };
</script>

<style scoped>
.github_projects {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-between;
}
.project {
  padding: 8px;
  text-align: left;
}
</style>
