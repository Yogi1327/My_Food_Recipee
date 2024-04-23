<script>
    let showIngredient = true
    let showInstructions = false

    function changeDisplay(type) {
        if (type === "ingredients") {
            showIngredient = true
            showInstructions = false
        }

        if (type === "instructions") {
            showIngredient = false
            showInstructions = true
        }

    }
    </script>

<!-- removed items-center -->
<div class="mx-auto py-8 grid grid-cols-1 md:grid-cols-2 gap-8 ">

    <div>
        <img src="/snacks/snack3.jpg" alt="Moong Dal Pakoras" class="w-full h-full object-cover mb-4">
    </div>
    <div class="border-t border-gray-200 pt-4 md:pt-0">
    <div>        <button on:click={() => changeDisplay("ingredients")}>Ingredients</button>        <button on:click={() => changeDisplay("instructions")}>Instructions</button></div>

        {#if showIngredient}
        <h1 class="text-3xl font-bold mb-4">Ingredients:</h1>
        <ul class="list-disc pl-6 mb-4">
            <li>1 cup split yellow lentils (moong dal)</li>
            <li>1 medium-sized onion, finely chopped</li>
            <li>2-3 green chilies, finely chopped (adjust according to your taste)</li>
            <li>2 tablespoons chopped fresh coriander leaves</li>
            <li>1 teaspoon ginger-garlic paste</li>
            <li>1/2 teaspoon cumin seeds</li>
            <li>1/2 teaspoon turmeric powder</li>
            <li>1/2 teaspoon red chili powder (adjust according to your spice preference)</li>
            <li>Salt to taste</li>
            <li>Oil for deep frying</li>
        </ul>
        {/if}
        {#if showInstructions}
        <h2 class="text-3xl font-bold mb-4">Instructions:</h2>
        <ol class="list-decimal pl-6 mb-4">
            <li><strong>Preparation of Moong Dal:</strong></li>
            <ul class="list-disc pl-6">
                <li>Wash the split yellow lentils (moong dal) thoroughly under running water until the water runs clear.</li>
                <li>Soak the washed moong dal in water for about 3-4 hours. This helps in easy grinding.</li>
                <li>After soaking, drain the water completely from the moong dal.</li>
            </ul>
            <li><strong>Grinding:</strong></li>
            <ul class="list-disc pl-6">
                <li>Transfer the soaked and drained moong dal into a blender or a food processor.</li>
                <li>Grind it into a coarse paste without adding water. The texture should be slightly grainy, not too smooth.</li>
            </ul>
            <li><strong>Making the Pakora Batter:</strong></li>
            <ul class="list-disc pl-6">
                <li>Transfer the ground moong dal into a mixing bowl.</li>
                <li>Add finely chopped onions, green chilies, ginger-garlic paste, chopped coriander leaves, cumin seeds, turmeric powder, red chili powder, and salt to taste.</li>
                <li>Mix all the ingredients well to form a thick batter. If the batter is too thick, you can add a tablespoon or two of water, but make sure it's not too runny.</li>
            </ul>
            <li><strong>Frying:</strong></li>
            <ul class="list-disc pl-6">
                <li>Heat oil for deep frying in a kadhai or deep frying pan over medium heat.</li>
                <li>Once the oil is hot, take small portions of the batter using your fingers or a spoon and carefully drop them into the hot oil.</li>
                <li>Fry the pakoras in batches, making sure not to overcrowd the pan.</li>
                <li>Fry the pakoras until they turn golden brown and crispy, flipping them occasionally for even cooking.</li>
                <li>Once done, remove the pakoras using a slotted spoon and drain the excess oil on paper towels.</li>
            </ul>
            <li><strong>Serving:</strong></li>
            <ul class="list-disc pl-6">
                <li>Serve the moong dal pakoras hot with green chutney, tamarind chutney, or ketchup.</li>
                <li>Enjoy your crispy and delicious moong dal pakoras as a tasty snack or appetizer!</li>
            </ul>
        </ol>
        {/if}
    </div>
</div>

<style>
    * {
        border: 1px solid black;
    }
</style>