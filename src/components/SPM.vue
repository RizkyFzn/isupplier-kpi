<template>
    <div class="wrapper">
        <div class="graph-wrapper">
            <h3 class="title">
                Supplier Performance Management
            </h3>
            <div class="graph">
                <vc-calendar is-expanded title-position="right"/>
                
            </div>
        </div>
        <div class="card-wrapper">
            <div class="card">
                <p>Total Perjanjian</p>
                <p>300</p>
            </div>
            <div class="card">
                <p>BAPP & BAST</p>
                <p>1.227.449.038.281</p>
            </div>
            <div class="card">
                <p>Approved</p>
                <p>227.449.038.281</p>
            </div>
            <div class="card">
                <p>Rata-rata tingkat kepuasan</p>
                <p>48 / 51</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
name: 'SPM',
data() {
    return {
      date: null,
      mode: "datetime",
    };
  },
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