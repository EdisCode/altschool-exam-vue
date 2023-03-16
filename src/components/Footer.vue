<template>
<section className="footer">
      <div>
        © {{currentDate()}} Service - Developed by
        <a href="https://github.com/EdisCode">Edikan Ekanem</a>
      </div>
    </section>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: 'Footer',
  methods: {
    currentDate() {
      const currentYear = new Date().getFullYear();
  const yearTxt = currentYear === 2022 ? "2022" : "2022 - " + currentYear;
      return yearTxt;
    }
  }
}
</script>