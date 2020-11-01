<template>
  <v-app>
    <v-form ref="form" class="containers" lazy-validation>
      <div class="title">Project</div>
      <v-divider></v-divider>
      <div class="container-1">
        <div class="text-field-block">
          <v-text-field
            class="text-field-1"
            label="Name"
            placeholder="Name"
            outlined
            required
          ></v-text-field>
        </div>

        <div class="container-2">
          <v-row>
            <v-col cols="12" sm="6">
              <v-text-field
                class="text-field-2"
                label="To"
                placeholder="To"
                outlined
                required
              ></v-text-field>
            </v-col>
            <v-col cols="12" sm="6">
              <v-text-field
                class="text-field-2"
                label="From"
                placeholder="From"
                outlined
                required
              ></v-text-field>
            </v-col>
          </v-row>
        </div>

        <div class="text-field-block">
          <v-select
            class="text-field-1"
            :items="items"
            label="Position"
            placeholder="Position"
            outlined
            required
          ></v-select>
        </div>

        <div class="text-field-block">
          <v-text-field
            class="text-field-1"
            label="Description"
            placeholder="Description"
            outlined
            required
          ></v-text-field>
        </div>

        <div class="text-field-block">
          <v-text-field
            class="text-field-1"
            label="Responsibilities"
            placeholder="Responsibilities"
            outlined
            required
          ></v-text-field>
        </div>
        <div class="text-field-block">
          <v-select
            class="text-field-1"
            :items="items"
            label="Team size"
            placeholder="Team size"
            outlined
            required
          ></v-select>
        </div>

        <div class="text-field-block">
          <v-text-field
            class="text-field-1"
            label="Technologies"
            placeholder="Technologies"
            outlined
            required
          ></v-text-field>
        </div>

        <v-btn color="#1867C0" class="mr-4 white--text btn"> SAVE </v-btn>
        <v-btn color="#F44336" class="mr-4 white--text btn"> DELETE </v-btn>
        <v-btn color="#FFFFFF" class="mr-4 black--text btn"> CANCEL </v-btn>
      </div>
    </v-form>
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},

  data: () => ({
    items: ["a", "b", "c", "d"],
  }),
};
</script>

<style lang="scss">
.title {
  margin-left: 24px;
  margin-top: 12px;
  margin-bottom: 12px;
}
.containers {
  position: relative;
  height: 686px;
  width: 800px;
  /* width: 41.7%; */
  left: 565px;
  /* left: 29.4%; */
  top: 303px;
  /* top: 15.8%; */
  border-radius: 5px;
  border: 1px solid #e5e5e5;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
.container-1 {
  position: absolute;
  left: 24px;
  top: 52px;
  width: 745px;
  right: 31px;
}
.text-field-block {
  width: 100%;
  margin-top: 21px;
  position: relative;
}
.text-field-1 {
  width: 100%;
  height: 56px;
  border-radius: 5px;
}

.container-2 {
  position: relative;
  width: 100%;
  margin-top: 9px;
  margin-bottom: -9px;
}
.text-field-2 {
  position: absolute;
  width: 360px;
  height: 56px;
}
.btn {
  float: right;
  position: absolute;
  width: 120px;
  height: 40px;
  background: #ffffff;
  border: 1px solid #e5e5e5;
  box-sizing: border-box;
  border-radius: 5px;
  margin-top: 20px;
}
</style>