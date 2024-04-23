<script>

    export let myImage
    export let snackName
    export let moreText
    console.log(myImage)

</script>


<div class="md:w-1/3 px-4 mb-8 myborder">
    <img class="rounded shadow-md w-full" src={myImage} alt="">
    <a href="../recipe">Name of snack</a>
    <h1 class="heading">{snackName}</h1>
    <p>{moreText}</p>
  </div>

  <style>

    .heading {

        font-size: 24px;
    }
p {
    color: lime;
}

.myborder {
    border: 2px solid orange;
}
</style>