<template>
  <div>
    <NuxtWelcome />
  </div>
</template>

<script setup lang="ts">
    import countryCodes, { CountryProperty } from 'country-codes-list'

    const countries = countryCodes.customList(
        CountryProperty.countryCode, '{countryNameEn}'
    )

    console.log(countries)
</script>
