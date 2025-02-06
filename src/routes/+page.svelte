<script lang="ts">
    import Grid from "$lib/components/Grid.svelte";
   import { GridFooter, type PagingData } from "$lib/index.js";

    let data;
    let companies = [
        {
            id: "1",
            name: "Company 1",
            catchPhrase: "Catch Phrase 1",
            city: "City 1",
            country: "Country 1",
            group: "A",
        },
        {
            id: "2",
            name: "Company 2",
            catchPhrase: "Catch Phrase 2",
            city: "City 2",
            country: "Country 2",
            group: "A",
        },
        {
            id: "3",
            name: "Company 3",
            catchPhrase: "Catch Phrase 3",
            city: "City 3",
            country: "Country 3",
            group: "B",
        },
        {
            id: "4",
            name: "Company 4",
            catchPhrase: "Catch Phrase 4",
            city: "City 4",
            country: "Country 4",
            group: "B",
        },
        {
            id: "5",
            name: "Company 5",
            catchPhrase: "Catch Phrase 5",
            city: "City 5",
            country: "Country 5",
            group: "C",
        },
        {
            id: "6",
            name: "Company 6",
            catchPhrase: "Catch Phrase 6",
            city: "City 6",
            country: "Country 6",
            group: "C",
        },
        {
            id: "7",
            name: "Company 7",
            catchPhrase: "Catch Phrase 7",
            city: "City 7",
            country: "Country 7",
            group: "C",
        },
        {
            id: "8",
            name: "Company 8",
            catchPhrase: "Catch Phrase 8",
            city: "City 8",
            country: "Country 8",
            group: "D",
        },
        {
            id: "9",
            name: "Company 9",
            catchPhrase: "Catch Phrase 9",
            city: "City 9",
            country: "Country 9",
            group: "E",
        },
        {
            id: "10",
            name: "Company 10",
            catchPhrase: "Catch Phrase 10",
            city: "City 10",
            country: "Country 10",
            group: "E",
        },
        {
            id: "11",
            name: "Company 11",
            catchPhrase: "Catch Phrase 11",
            city: "City 11",
            country: "Country 11",
            group: "E",
        },
        {
            id: "12",
            name: "Company 12",
            catchPhrase: "Catch Phrase 12",
            city: "City 12",
            country: "Country 12",
            group: "E",
        },
        {
            id: "13",
            name: "Company 13",
            catchPhrase: "Catch Phrase 13",
            city: "City 13",
            country: "Country 13",
            group: "E",
        },
        {
            id: "14",
            name: "Company 14",
            catchPhrase: "Catch Phrase 14",
            city: "City 14",
            country: "Country 14",
            group: "E",
        },
        {
            id: "15",
            name: "Company 15",
            catchPhrase: "Catch Phrase 15",
            city: "City 15",
            country: "Country 15",
            group: "E",
        }
    ];

    let columns = ["", "id", "name", "catchPhrase", "city", "country", "group"];
    let groupBy = $state("");

    let paging = $state({
        itemsPerPage: 5,
        currentPage: 1,
        itemsPerPageOptions: [5, 10, 15],
    });
</script>

<label for="groupBySelection">Group By:</label>
<select id="groupBySelection" bind:value={groupBy}>
    {#each columns as col}
        <option value={col}>{col}</option>
    {/each}
</select>

<br /><br />

<Grid data={companies} {groupBy} {paging}/>

<GridFooter bind:paging />