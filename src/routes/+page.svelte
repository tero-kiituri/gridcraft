<script lang="ts">
    import Grid from '$lib/components/Grid.svelte';

    export let data;
    let companies = [
        {
            id: "1",
            name: "Company 1",
            catchPhrase: "Catch Phrase 1",
            city: "City 1",
            country: "Country 1",
            group: "A"
        },
        {
            id: "2",
            name: "Company 2",
            catchPhrase: "Catch Phrase 2",
            city: "City 2",
            country: "Country 2",
            group: "A"
        },
        {
            id: "3",
            name: "Company 3",
            catchPhrase: "Catch Phrase 3",
            city: "City 3",
            country: "Country 3",
            group: "B"
        },
        {
            id: "4",
            name: "Company 4",
            catchPhrase: "Catch Phrase 4",
            city: "City 4",
            country: "Country 4",
            group: "B"
        },
        {
            id: "5",
            name: "Company 5",
            catchPhrase: "Catch Phrase 5",
            city: "City 5",
            country: "Country 5",
            group: "C"
        },
        {
            id: "6",
            name: "Company 6",
            catchPhrase: "Catch Phrase 6",
            city: "City 6",
            country: "Country 6",
            group: "C"
        },
        {
            id: "7",
            name: "Company 7",
            catchPhrase: "Catch Phrase 7",
            city: "City 7",
            country: "Country 7",
            group: "C"
        },
        {
            id: "8",
            name: "Company 8",
            catchPhrase: "Catch Phrase 8",
            city: "City 8",
            country: "Country 8",
            group: "D"
        },
        {
            id: "9",
            name: "Company 9",
            catchPhrase: "Catch Phrase 9",
            city: "City 9",
            country: "Country 9",
            group: "E"
        },
        {
            id: "10",
            name: "Company 10",
            catchPhrase: "Catch Phrase 10",
            city: "City 10",
            country: "Country 10",
            group: "E"
        }
    ];
</script>

<Grid data={companies} />
