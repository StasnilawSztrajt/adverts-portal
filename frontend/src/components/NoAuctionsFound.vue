<template>
  <div id="NoAdvertsFound" class="text-gray-400 text-xl sm:text-2xl mt-10">
    <h1 class="text-8xl mb-5">:(</h1>
    <h2 class="mb-3 sm:mb-2">
      Nie znaleźliśmy ogłoszeń dla zapytania <span class="font-semibold">"{{ searchInputItem }}"</span>
      <span v-if="searchInputLocation !== ''">
        dla lokalizacji <span class="font-semibold">"{{ searchInputLocation }}"</span>
      </span>.
    </h2>
    <h2>Sprawdź poprawność wyszukiwanej frazy, lub użyj bardziej ogólnego zapytania.</h2>
  </div>
</template>
<script>
export default {
  props: {
    searchInputItem: {
      type: String
    },
    searchInputLocation: {
      type: String
    },
  },
}
</script>