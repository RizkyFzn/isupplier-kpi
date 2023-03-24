<template>
    <div class="content-wrapper">
        <!-- Sidebar -->
        <div class="sidebar">
            <p class="title">Date Range</p>
            <div>
                <DateRange/>
                <!-- <DatePicker/> -->
            </div>

            <p class="title">Grafik</p>
            <div class="button-wrapper">
                <button v-bind:class="{active: menu === 'sap'}" v-on:click="menu = 'sap'">Register to SAP</button>
                <button v-bind:class="{active: menu === 'k3l'}" v-on:click="menu = 'k3l'">Praqualifikasi K3L</button>
                <button v-bind:class="{active: menu === 'kplh'}" v-on:click="menu = 'kplh'">Praqualifikasi KPLH</button>
                <button v-bind:class="{active: menu === 'k3lkplh'}" v-on:click="menu = 'k3lkplh'">Praqualifikasi K3L & KPLH</button>
                <button v-bind:class="{active: menu === 'csi'}" v-on:click="menu = 'csi'">CSI Score</button>
                <button v-bind:class="{active: menu === 'ssi'}" v-on:click="menu = 'ssi'">SSI</button>
                <button v-bind:class="{active: menu === 'spm'}" v-on:click="menu = 'spm'">SPM</button>
            </div>
            
            <p class="title">Tipe Request</p>

            <select name="request" id="request">
                    <option value="">All</option>
                    <option value="">1</option>
                    <option value="">2</option>
            </select>
        </div>
        <!-- End of Sidebar -->

        <!-- body content -->
        <div class="body-text">
            <div v-if="menu === 'sap'">
                <RegisterSap/>
            </div>
            <div v-else-if="menu === 'k3l'">
                <K3L/>
            </div>
            <div v-else-if="menu === 'kplh'">
                <KPLH/>
            </div>
            <div v-else-if="menu === 'csi'">
                <CsiScore/>
            </div>
            <div v-else-if="menu === 'ssi'">
                <SSI/>
            </div>
            <div v-else-if="menu === 'spm'">
                <SPM/>
            </div>
        </div>
        <!-- End of body content -->
    
        
        
    </div>
</template>

<script>
// import DatePicker from './DatePicker.vue';
import CsiScore from './CsiScore.vue'
import K3L from './K3L.vue'
import KPLH from './KPLH.vue'
import RegisterSap from './RegisterSAP.vue'
import SPM from './SPM.vue'
import SSI from './SSI.vue'
import DateRange from './DateRange.vue'

export default {
name: 'MainContent',
components: {
    RegisterSap,
    SPM,
    // DatePicker
    DateRange,    
    SSI,
    K3L,
    KPLH,
    CsiScore
},
data: function () {
    return {
        menu: 'sap',
        open: false,
    }
} 
}
</script>

<style scoped>
.content-wrapper {
    display: flex;
    flex-direction: row;
}
.title {
    color: red;
    font-weight: 600;
}

.active {
    background-color: red;
    color: white;
}

.button-wrapper {
    display: flex;
    flex-direction: column;
    gap: .4rem;
    
}

button {
    text-align: left;
    background-color: white;
    padding: .4rem;
    color: red;
    border: 1px solid red;
}

button:hover {
    background-color: red;
    color: white;
    cursor: pointer;
}

.sidebar {
    height: 80vh;
    width: 250px;
    position: relative;
    left: 0;
    top: 0;
    padding-top: 15px;
    border-right: 2px solid gray;
    /* background-color: lightblue; */
    padding-left: 15px;
    padding-right: 25px;
}

select {
    width: 12rem;
}

.body-text {
    /* display: flex; */
    /* align-items: center; */
    width: 100%;
    height: 100%;
    padding: 20px;
    /* font-size: 18px; */
    background-color: rgb(241, 208, 213);
}
</style>
