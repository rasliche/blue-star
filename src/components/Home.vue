<template lang="html">
    <div class="container mx-auto font-sans">
        <div class="tracks flex py-8">
            <div class="blue-star text-center flex-1">
                <h3 @mouseenter="blueStar = !blueStar" @mouseleave="blueStar = !blueStar" :class="{'bs-border': blueStar}">Diving</h3>
            </div>
            <div class="naturalist text-center flex-1">
                <h3 @mouseenter="naturalist = !naturalist" @mouseleave="naturalist = !naturalist" :class="{'n-border': naturalist}">Naturalist</h3>
            </div>
            <div class="team-ocean text-center flex-1">
                <h3 @mouseenter="teamOcean = !teamOcean" @mouseleave="teamOcean = !teamOcean" :class="{'to-border': teamOcean}">Team OCEAN</h3>
            </div>
            <div class="marine-debris text-center flex-1">
                <h3 @mouseenter="marineDebris = !marineDebris" @mouseleave="marineDebris = !marineDebris" :class="{'md-border': marineDebris}">Marine Debris Cleanup</h3>
            </div>
        </div>

        <div class="modules flex flex-wrap">
            <p class="h-12 w-1/5 text-center py-2"  :class="{'n-border': naturalist, 'bs-border': blueStar, 'to-border': teamOcean, 'md-border': marineDebris}">101</p>
            <p class="w-1/5 text-center py-2" :class="{'bs-border': blueStar, 'to-border': teamOcean, 'n-border': naturalist, 'md-border': marineDebris}">Rules/Regs</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Interpretation</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Marine Debris</p>
            <p class="w-1/5 text-center py-2" :class="{'bs-border': blueStar, 'n-border': naturalist, 'md-border': marineDebris}">Seagrass I</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar, 'border-green-light': naturalist, 'border-2': naturalist, 'rounded-lg': naturalist}">Corals I</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar, 'border-green-light': naturalist, 'border-2': naturalist, 'rounded-lg': naturalist}">Mangroves I</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar, 'border-green-light': naturalist, 'border-2': naturalist, 'rounded-lg': naturalist}">Maritime Heritage Resources I</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Diver Management</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Seagrass II</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Corals II</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Mangroves II</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Maritime Heritage Resources II</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Current Science I</p>
            <p class="w-1/5 text-center py-2">Seagrass III</p>
            <p class="w-1/5 text-center py-2">Corals III</p>
            <p class="w-1/5 text-center py-2">Mangroves III</p>
            <p class="w-1/5 text-center py-2">Maritime Heritage Resources III</p>
            <p class="w-1/5 text-center py-2">Current Science II</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Zones</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Marine Life</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Reporting/Response</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Lionfish</p>
            <p class="w-1/5 text-center py-2">Current Science III</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Buoys</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Hazardous Marine Life</p>
            <p class="w-1/5 text-center py-2">Vessels</p>
            <p class="w-1/5 text-center py-2" :class="{'border-blue-light': blueStar, 'border-2': blueStar, 'rounded-lg': blueStar}">Lionfish II</p>
            <p class="w-1/5 text-center py-2">Safety</p>
            <p class="w-1/5 text-center py-2">Volunteer Requirements</p>
            <p class="w-1/5 text-center py-2"></p>
            <p class="w-1/5 text-center py-2"></p>
            <p class="w-1/5 text-center py-2"></p>
            <p class="w-1/5 text-center py-2"></p>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            blueStar: false,
            naturalist: false,
            teamOcean: false,
            marineDebris: false
        }
    }
}
</script>

<style lang="css">
</style>
