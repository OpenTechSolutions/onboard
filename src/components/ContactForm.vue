<template>
  <div class="shadow rounde md:w-6/12 w-11/12 m-auto mt-10 p-5 mb-10 bg-gray-100">
    <h1 class="text-2xl font-bold mb-5">Contact Us</h1>
    <input type="text" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline my-2" name="name" placeholder="Name">
    <input type="email" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline my-2" name="email" placeholder="Email">
    <textarea name="message" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline my-2" id="msg" cols="30" rows="7" placeholder="Enter message"></textarea>
    <button type="submit" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline">Submit</button>
  </div>
</template>

<script>
export default {
  name: 'ConatForm'
}
</script>

<style>
textarea{
  resize: none !important;
}
</style>
