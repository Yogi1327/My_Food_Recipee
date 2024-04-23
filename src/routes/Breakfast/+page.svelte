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
      
  
    ]
  </script>

<main>
  
    <div class="container mx-auto border border-indigo-500 px-4">    

        <div>


            <div class="container mx-auto">
           
              
    
             
                <div class="flex justify-center">
                    <a href="src/routes/Breakfast" class="block text-center bg-gray-100 py-8"></a>
                    <div class="w-full md:w-2/3 lg:w-1/2">
                      
                        <h2 class="text-3xl font-bold mb-4">Breakfast</h2>
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
        
                </div>
        
              </section>
        
          
          
            </div>
        
          </main>
            
