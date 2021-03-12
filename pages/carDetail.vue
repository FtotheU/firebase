<template>
  <v-row justify="center">
    <v-col cols="12" sm="12">
      <h1 class="text-center">รายละเอียดรถยนต์</h1>
    </v-col>
    <v-col cols="12" sm="5">
      <v-card rounded="lg"
        ><v-img
          class="white--text align-end"
          src="https://picsum.photos/id/11/500/300"
          align="center"
        >
        </v-img
      ></v-card>
    </v-col>
    <v-col cols="12" sm="5"
      ><v-card rounded="lg" min-height="400" color="white">
        <v-toolbar color="light-blue" dark dense flat>
          <v-toolbar-title class="body-2"> ชื่อยี่ห้อรถยนต์ </v-toolbar-title>
        </v-toolbar>
        <v-card-subtitle>001</v-card-subtitle>
        <v-card-text class="text--primary">
          <div class="dt">
            <v-icon class="ic" x-large> mdi-bitcoin </v-icon> ราคาเช่า 5555 บาท
          </div>
          <div class="dt">
            <v-icon class="ic" x-large> mdi-car-seat </v-icon> 555
          </div>
          <div class="dt">
            <v-icon class="ic" x-large> mdi-treasure-chest </v-icon>555
          </div>
          <div class="dt">
            <v-icon class="ic" x-large>mdi-car</v-icon> 555
          </div> </v-card-text
        ><v-card-actions>
          <v-btn color="yellow darken-2" rounded block> ทำสัญญาเช่า </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>

    <v-col cols="12" sm="12"> </v-col>
  </v-row>
</template>

<script></script>
<style>
.ic {
  margin-right: 2rem;
}
.dt {
  margin: 0.8rem;
}
</style>
