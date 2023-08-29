<template>
  <tr>
    <td class="px-6">
      <div class="flex items-center space-x-3">
        <div class="avatar">
          <div class="mask mask-squircle w-12 h-12">
            <img
              src="/tailwind-css-component-profile-2@56w.png"
              alt="Avatar Tailwind CSS Component"
            />
          </div>
        </div>
        <div>
          <div class="font-bold">{{ person.fname }}</div>
          
        </div>
      </div>
    </td>
    <td>
      {{ person.company }}
      <br />
      <span class="badge-lg sm:badge badge badge-ghost text-xs md:text-base    ">{{ person.job }}</span>
    </td>
  </tr>
</template>


<script>

export default {
  components: "Row",
  props: ['person']
}

</script>