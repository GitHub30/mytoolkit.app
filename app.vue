<script setup>
import { ref } from 'vue'

const drawer = ref(null)

function gotoTop() {
  location = '.'
}
</script>
<template>
  <NuxtLayout>
    <v-app>
      <v-app-bar>
        <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
        <v-app-bar-title @click="gotoTop">My Toolkit Online</v-app-bar-title>
        <v-btn href="https://github.com/GitHub30/mytoolkit.app" target="_blank" icon="mdi-github"></v-btn>
      </v-app-bar>

      <v-navigation-drawer v-model="drawer">
        <v-list>
          <v-list-item title="Google Search" to="google-search"></v-list-item>
          <v-list-item title="Password Generator" to="password-generator"></v-list-item>
          <v-list-item title="Passphrase Generator" to="passphrase-generator"></v-list-item>
          <v-list-item title="URL Shortener" to="url-shortener"></v-list-item>
          <v-list-item title="UUID Generator" to="uuid-generator"></v-list-item>
          <v-list-item title="file.gz Extractor" to="gz-extractor"></v-list-item>
          <v-list-item title="TOTP Generator" to="totp-generator"></v-list-item>
          <v-list-item title="CSR Generator" to="csr-generator"></v-list-item>
          <v-list-item title="CSR Decoder" to="csr-decoder"></v-list-item>
          <v-list-item title="CRT Decoder" to="crt-decoder"></v-list-item>
          <v-list-item title="Sectigo Token" to="sectigo-token"></v-list-item>
          <v-list-item title="SSH Key Generator" to="ssh-key-generator"></v-list-item>
          <v-list-item title="A Lookup" to="a-lookup"></v-list-item>
          <v-list-item title="AAAA Lookup" to="aaaa-lookup"></v-list-item>
          <v-list-item title="CNAME Lookup" to="cname-lookup"></v-list-item>
          <v-list-item title="TXT Lookup" to="txt-lookup"></v-list-item>
          <v-list-item title="NS Lookup" to="ns-lookup"></v-list-item>
          <v-list-item title="PTR Lookup" to="ptr-lookup"></v-list-item>
          <v-list-item title="ANY Lookup" to="any-lookup"></v-list-item>
          <v-list-item title="CAA Lookup" to="caa-lookup"></v-list-item>
          <v-list-item title="MX Lookup" to="mx-lookup"></v-list-item>
          <v-list-item title="NAPTR Lookup" to="naptr-lookup"></v-list-item>
          <v-list-item title="SOA Lookup" to="soa-lookup"></v-list-item>
          <v-list-item title="SRV Lookup" to="srv-lookup"></v-list-item>
          <v-list-item title="Reverse IP Lookup" to="reverse-ip-lookup"></v-list-item>
          <v-list-item title="Whois" to="whois"></v-list-item>
          <v-list-item title="MD5" to="md5"></v-list-item>
          <v-list-item title="SHA1" to="sha1"></v-list-item>
          <v-list-item title="SHA256" to="sha256"></v-list-item>
          <v-list-item title="SHA384" to="sha384"></v-list-item>
          <v-list-item title="SHA512" to="sha512"></v-list-item>
          <v-list-item title="SHA512/224" to="sha512-224"></v-list-item>
          <v-list-item title="SHA512/256" to="sha512-256"></v-list-item>
          <v-list-item title="HMAC" to="hmac"></v-list-item>
          <v-list-item title="Count Lines" to="count-lines"></v-list-item>
          <v-list-item title="Replace text" to="replace-text"></v-list-item>
          <v-list-item title="Remove JS key quotes" to="remove-key-quotes"></v-list-item>
          <v-list-item title="Video Frame Picker" to="video-frame-picker"></v-list-item>
          <v-list-item title="unserialize.php" to="unserialize-php"></v-list-item>
          <v-list-item title="Screen Wake Lock" to="wake-lock"></v-list-item>
          <v-list-item title="OCR" to="ocr"></v-list-item>
          <v-list-item title="Web MAIL" to="mail"></v-list-item>
          <v-list-item title="Web FTP" to="ftp"></v-list-item>
          <v-list-item title="ふりがな（ルビ）" to="furigana"></v-list-item>
          <v-list-item title="形態素解析" to="morphological-analysis"></v-list-item>
          <v-list-item title="キーフレーズ抽出" to="keyword-extraction"></v-list-item>
          <v-list-item title="Website Availability" to="website-availability"></v-list-item>
        </v-list>
      </v-navigation-drawer>

      <v-main>
        <NuxtPage />
      </v-main>
    </v-app>
  </NuxtLayout>
</template>
<style>
html {
  overflow-y: auto;
}
</style>