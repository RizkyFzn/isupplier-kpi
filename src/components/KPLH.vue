<template>
    <div class="wrapper">

        <div class="graph-wrapper">
            <h3 class="title">
                SLA Performance
            </h3>
            <div class="graph">
                <Date/>
            </div>
        </div>
        <div class="card-wrapper">
            <div class="card">
                <p>Total Request</p>
                <p>250</p>
            </div>
            <div class="card">
                <p>Penilaian Manual</p>
                <p>200</p>
            </div>
            <div class="card">
                <p>Penilaian Oleh Sistem</p>
                <p>25</p>
            </div>
            <div class="card">
                <p>Belum dinilai</p>
                <p>25</p>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: "KPLH"
}

</script>

<style scoped>

    .graph-wrapper {
        width: 70%;
        min-height: 50vh;
        /* height: 100vh; */
        text-align: center;
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        background-color: white;
        /* border: 1px solid cyan; */
    }
    .wrapper {
        /* border: 1px solid red; */
        width: 100%;
        display: flex;
        justify-content: space-between;
        flex-direction: row;
        flex-wrap: wrap;
        /* border: 2px solid blue; */
        gap: 2.5rem;
    }

    .graph {
        
    }

    .card-wrapper {
        width: 25%;
        /* border: 1px solid red; */
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }

    .card {
        background-color: white;
        padding: .5rem;
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
    }

</style>