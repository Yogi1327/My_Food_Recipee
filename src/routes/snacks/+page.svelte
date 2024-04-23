<script>
  import GridBox from "$lib/components/GridBox.svelte";

  let myGridBoxes = [
    {
      imageUrl: "./snacks/snack3.jpg",
      snackName: "Nectarine",
      otherText: "Pretty good"
    },
    {
      imageUrl: "./snacks/snack1.jpg",
      snackName: "Lemon",
      otherText: "Too sour"
    },
    {
      imageUrl: "./snacks/snack2.jpg",
      snackName: "Grapes",
      otherText: "Perfect"
    },
    {
      imageUrl: "./snacks/snack3.jpg",
      snackName: "Nectarine",
      otherText: "Pretty good"
    },
    {
      imageUrl: "./snacks/snack1.jpg",
      snackName: "Lemon",
      otherText: "Too sour"
    },
    {
      imageUrl: "./snacks/snack2.jpg",
      snackName: "Grapes",
      otherText: "Perfect"
    },
    {
      imageUrl: "./snacks/snack3.jpg",
      snackName: "Nectarine",
      otherText: "Pretty good"
    },
    {
      imageUrl: "./snacks/snack1.jpg",
      snackName: "Lemon",
      otherText: "Too sour"
    },
    {
      imageUrl: "./snacks/snack2.jpg",
      snackName: "Grapes",
      otherText: "Perfect"
    },
    {
      imageUrl: "./snacks/snack3.jpg",
      snackName: "Nectarine",
      otherText: "Pretty good"
    },
    {
      imageUrl: "./snacks/snack1.jpg",
      snackName: "Lemon",
      otherText: "Too sour"
    },
    {
      imageUrl: "./snacks/snack2.jpg",
      snackName: "Grapes",
      otherText: "Perfect"
    },

  ]
</script>



<main>
  
    <div class="container mx-auto border border-indigo-500 px-4">    
     <!--  <h1 class="font-bold text-5xl">Snacks Gallery</h1> -->

      <!-- <img src="./snacks/snack3.jpg" alt="test" />
  
      <section class="py-8 px-4">
        <div class="flex flex-wrap mx-4">
          <div class="md:w-1/2 px-4 mb-8 md:mb-0"><img class="rounded shadow-md" src="./snacks/snack1.jpg" alt="snack1"></div>
          <div class="md:w-1/2 px-4 mb-8 md:mb-0"><img class="rounded shadow-md" src="./snacks/snack2.jpg" alt="snack2"></div>
        </div>
      </section> -->

      <div>


        <div class="container mx-auto">
      
          

         
            <div class="flex justify-center">
                <a href="src/routes/Curries/+page.svelte" class="block text-center bg-gray-100 py-8"></a>
                <div class="w-full md:w-2/3 lg:w-1/2">
                  
                    <h2 class="text-3xl font-bold mb-4">Bites & Delights</h2>
                    <hr class="border-t-2 border-gray-300 mb-8">
                </div>
            </div>
        </div>

  
      <section class="pt-8 px-4">

        <!-- container for snack containers -->
        <div class="flex flex-wrap mx-4">

          {#each myGridBoxes as item}
            <GridBox myImage={item.imageUrl} snackName={item.snackName}  moreText={item.otherText}/>
          {/each}





<!-- 
          <GridBox myImage="" snackName="chips"  moreText="rated 10/10"/>

          <GridBox myImage="./snacks/snack3.jpg" snackName="ice-cream"  moreText="rated 10/10"/>
          <GridBox myImage="./snacks/snack3.jpg" snackName="chips"  moreText="rated 10/10"/>
          <GridBox myImage="./snacks/snack3.jpg" snackName="chips"  moreText="rated 10/10"/> -->

          <!-- <div class="md:w-1/3 px-4 mb-8">
            <img class="rounded shadow-md w-full" src="./snacks/snack3.jpg" alt="">
            <a href="../recipe">Name of snack</a>
            <p>More text</p>
            <p>Even more text</p>
          </div> 
     
          <div class="md:w-1/3 px-4 mb-8"><img class="rounded shadow-md w-full h-full" src="https://source.unsplash.com/random/1280x720" alt=""></div>
       
          
        
        
          <div class="md:w-1/3 px-4 mb-8"><img class="rounded shadow-md w-full h-full" src="./snacks/snack3.jpg" alt=""></div>
          <div class="md:w-1/3 px-4 mb-8"><img class="rounded shadow-md w-full h-full" src="./snacks/snack2.jpg" alt=""></div>

          <div class="md:w-1/3 px-4 mb-8"><img class="rounded shadow-md w-full h-full" src="https://source.unsplash.com/random/1280x720" alt=""></div>
          <div class="md:w-1/3 px-4 mb-8"><img class="rounded shadow-md w-full h-full" src="https://source.unsplash.com/random/1280x720" alt=""></div> -->
         
        </div>
     
      </section>

  
  
    </div>

  </main>
