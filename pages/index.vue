<template>
  <v-container
    ><v-row justify="center" style="margin-top: 5%">
      <v-col cols="12" sm="6" style="margin-top: 5%">
        <h3>ยินดีต้อนรับสู่</h3>
        <h1 style="color: #4caf50">SKYCAR</h1>
        <h4>เว็บไซต์เช่ารถยนต์รายวันที่ดีที่สุดในเชียงใหม่</h4>
      </v-col>
      <v-col cols="12" sm="4">
        <h4>ให้เรารู้ข้อมูลของคุณ ไม่ต้องห่วงมันจะเป็นความลับ</h4>
        <v-divider class="dvd" />
        <v-subtitle>ชื่อและนามสกุล</v-subtitle>
        <v-row>
          <v-col sm="6">
            <v-text-field
              label="ชื่อ"
              placeholder="ชื่อ"
              solo
              dense
              rounded
              style="margin-top: 0.5rem"
            ></v-text-field
          ></v-col>
          <v-col sm="6">
            <v-text-field
              label="นามสกุล"
              placeholder="นามสกุล"
              solo
              dense
              rounded
              style="margin-top: 0.5rem"
            ></v-text-field
          ></v-col>
        </v-row>
        <v-subtitle>เบอร์โทรศัพท์</v-subtitle>
        <v-text-field
          label="เบอร์โทรศัพท์"
          placeholder="เบอร์โทรศัพท์"
          solo
          dense
          rounded
          style="margin-top: 0.5rem"
        ></v-text-field>
        <v-subtitle>เลขประจำตัวประชาชน</v-subtitle>
        <v-text-field
          label="เลขประจำตัวประชาชน"
          placeholder="เลขประจำตัวประชาชน"
          solo
          dense
          rounded
          style="margin-top: 0.5rem"
        ></v-text-field>
        <v-subtitle>อีเมล</v-subtitle>
        <v-text-field
          label="อีเมล"
          placeholder="อีเมล"
          solo
          dense
          rounded
          style="margin-top: 0.5rem"
        ></v-text-field>
        <v-list-item-subtitle>รหัสผ่าน</v-list-item-subtitle>
        <v-text-field
          label="รหัสผ่าน"
          placeholder="รหัสผ่าน"
          solo
          dense
          rounded
          style="margin-top: 0.5rem"
        ></v-text-field>
        <v-list-item-subtitle>ยืนยันรหัสผ่าน</v-list-item-subtitle>
        <v-text-field
          label="รหัสผ่าน"
          placeholder="รหัสผ่าน"
          solo
          dense
          rounded
          style="margin-top: 0.5rem"
        ></v-text-field>
        <v-divider class="dvd" />
        <h4>ตรวจสอบข้อมูลให้ถูกต้อง เราจะเก็บบันทึกข้อมูลของคุณ</h4>
        <div class="text-center">
          <v-btn
            @click="snackbar = true"
            rounded
            color="green"
            dark
            style="margin-top: 0.5rem"
          >
            สมัครสมาชิก
          </v-btn>

          <v-snackbar v-model="snackbar" :timeout="timeout">
            {{ text }}

            <template v-slot:action="{ attrs }">
              <v-btn color="red" text v-bind="attrs" @click="snackbar = false">
                Close
              </v-btn>
            </template>
          </v-snackbar>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    snackbar: false,
    text: 'ยินดีที่ได้รู้จัก เลือกรถที่คุณต้องการสิ',
    timeout: 2000,
  }),
}
</script>
<style>
.dvd {
  margin-top: 1rem;
  margin-bottom: 1rem;
}
</style>
