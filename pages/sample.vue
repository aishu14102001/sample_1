<template>
    <div>
      <h1>Media Content Page</h1>
      <div class="media-list">
        <!-- Display a list of media items with placeholder content (Lorem Ipsum) -->
        <div v-for="mediaItem in mediaItems" :key="mediaItem.id" class="media-item">
          <!-- Replace with your media content -->
          <p>{{ mediaItem.content }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        mediaItems: [
          { id: 1, content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.' },
          { id: 2, content: 'Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.' },
          { id: 3, content: 'Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris.' },
          // Add more media items with Lorem Ipsum text or other placeholder content as needed
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  /* Add your custom CSS styles here */
  .media-list {
    display: flex;
    flex-wrap: wrap;
  }
  
  .media-item {
    margin: 10px;
    width: 200px;
    height: 200px;
    border: 1px solid #ccc;
    padding: 10px;
    box-sizing: border-box;
  }
  </style>
  