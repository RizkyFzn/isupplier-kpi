<template>
    <div class="wrapper">

        <div class="graph-wrapper">
            <h3 class="title">
                Supplier Satisfaction Index
            </h3>
            <div class="graph">
                Graph
            </div>
        </div>
        <div class="card-wrapper">
            <div class="card">
                <p>Total PO</p>
                <p>300</p>
            </div>
            <div class="card">
                <p>Total PO Amount</p>
                <p>1.227.449.038.281</p>
            </div>
            <div class="card">
                <p>Top 10 Vendor PO Amount</p>
                <p>227.449.038.281</p>
            </div>
            <div class="card">
                <p>User Confirmation</p>
                <p>48 / 51</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
name: 'SSI',
// components: {
//     RegisterAriba
//     }
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