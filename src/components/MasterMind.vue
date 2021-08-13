<template>
    <div>
    <div id="gamingBoard">
        <div class="row">
            <span class="guessingPegs"></span>
            <span class="checkingPegs"></span>
        </div>
        <button type="submit">button</button> 
    </div>

    <div id="v-model-select" class="demo">
        <select>
            <option value="">Please select one</option>
            <option selected>blue</option>
            <option>green</option>
            <option>yellow</option>
            <option>orange</option>
            <option>pink</option>
        </select>
    </div>
<span>Selected: {{ selected }}</span>

    <select name="cars" id="cars">
        <option value="volvo">Volvo</option>
        <option value="saab">Saab</option>
        <option selected value="mercedes">Mercedes</option>
        <option value="audi">Audi</option>
    </select>


    </div>
</template>

<script>
export default {
    methods: {},
    data () {return{
        secretCode: [],
        guesses: [],
        selected: '',
    }}

}
</script>

<style>

    #gamingBoard {
        height: 612px;
        width: 256px;
        border: 2px;
        background-color: green 
    }

    .row {
        height: 50px;
        width: 256px;
        border: 1px black;
    }

    .guessingPegs {
        height: 50px;
        width: 50px;
        background-color: white;
        border: 1px black;
        border-radius: 50%;
        display: inline-block;
    }

    .checkingPegs {
        min-height: 25px;
        min-width: 25px;
        background-color: gold;
        border: 1px black;
        border-radius: 50%;
        display: inline-block;
    }
</style>