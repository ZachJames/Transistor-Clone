<template>
  <div class="px-6 pt-10 relative">
    <div class="absolute inset-x-0 top-0">
      <div class="w-40 bg-navy-dark mx-auto flex text-navy-light rounded overflow-hidden mb-4">
        <span
          class="rounded text-navy-darker bg-white py-1 uppercase text-center w-1/2 text-xs font-bold tracking-wide"
        >Monthly</span>
        <span
          class="rounded py-1 uppercase text-center w-1/2 text-xs font-bold tracking-wide hover:bg-navy"
        >Yearly</span>
      </div>
    </div>
    <plan-card
      name="Starter"
      monthly="19"
      :selected="true"
      :features="
        ['10,000 downloads / month',
        'Unlimited shows and episodes',
        'Analytics, teams, and more…'
        ]"
    ></plan-card>
    <plan-card
      name="Professional"
      monthly="49"
      :selected="false"
      :features="
        ['45,000 downloads / month',
        'Unlimited shows and episodes',
        'Analytics, teams, and more…'
        ]"
    ></plan-card>
    <plan-card
      name="Small Business"
      monthly="99"
      :selected="false"
      :features="
        ['150,000 downloads / month',
        'Unlimited shows and episodes',
        'Analytics, teams, and more…'
        ]"
    ></plan-card>
  </div>
</template>

<script>
import PlanCard from './PlanCard'

export default {
  name: "plan-selector",
  components: {
    PlanCard
  },
  props: [],
  data() {
    return {}
  },
  methods: {},
}
</script>
