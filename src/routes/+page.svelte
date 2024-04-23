

<script>
     import { AccordionItem, Accordion } from 'flowbite-svelte';
    import { Carousel } from 'flowbite-svelte';
    import images from './images.json';


  </script>


<!-- <Button>Recipes <ChevronDownOutline class="w-3 h-3 ms-2 text-white dark:text-white" /></Button> -->


<main>
  <div class="container mx-auto border border-indigo-500 px-4">    

<section class="pt-8 px-4">
  <div >
 <Carousel class="sm:mx-2.5 md:mx-5 lg:mx-10" {images} duration="3000" />

   </div>
  </section>

  <Accordion>
    <AccordionItem>
      <span slot="header">Culinary Preamble </span>
      <p class="mb-2 text-gray-500 dark:text-gray-400">Indian cuisine is renowned worldwide for its rich flavors, vibrant colors, and diverse range of ingredients. As one of the oldest and most culturally diverse culinary traditions, Indian food reflects the country's vast history, geography, and cultural influences. From spicy curries to fragrant rice dishes and mouthwatering sweets, Indian cuisine offers a gastronomic journey that tantalizes the taste buds and captivates the senses.</p>
      <p class="text-gray-500 dark:text-gray-400">
        One of the defining characteristics of Indian food is its extensive use of spices and herbs, which are skillfully blended to create complex layers of flavor. These spices, including cumin, coriander, turmeric, and cardamom, not only enhance the taste of dishes but also contribute to their vibrant hues. Each region of India boasts its own unique spice blends and cooking techniques, resulting in a diverse array of culinary styles and specialties.
      </p>
      <p class="text-gray-500 dark:text-gray-400">
        The diversity of Indian cuisine is also reflected in its regional variations, with each state and community offering its own distinct culinary traditions and specialties. For example, the fiery dishes of the south contrast with the creamy curries of the north, while the coastal regions showcase an abundance of seafood-based delicacies. Moreover, the influence of historical migrations, trade routes, and cultural exchanges has enriched Indian cuisine with elements from Persian, Mughal, Portuguese, and British culinary traditions.
      </p>
      <!-- <p class="text-gray-500 dark:text-gray-400">
        Check out this guide to learn how to <a href="/" target="_blank" rel="noreferrer" class="text-blue-600 dark:text-blue-500 hover:underline"> get started </a>
        and start developing websites even faster with components on top of Tailwind CSS.
      </p> -->
    </AccordionItem>
  
  </Accordion>

  </div>
</main>