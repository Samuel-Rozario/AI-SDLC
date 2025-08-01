// Code for creating and publishing new content (posts)

class User {
  constructor(name) {
    this.name = name;
    this.isLoggedIn = false;
  }

  login() {
    this.isLoggedIn = true;
  }

  createPost(content, media) {
    if (!this.isLoggedIn) {
      console.log("User is not logged in.");
      return;
    }

    if (!content.trim()) {
      console.log("Validation Error: Content cannot be empty.");
      return;
    }

    const newPost = {
      content: content,
      media: media
    };

    this.publishPost(newPost);
  }

  publishPost(post) {
    // Logic to publish the post on user's profile and public feed
    console.log("New post published:", post);
  }
}

// Usage
const currentUser = new User("Alice");
currentUser.login();

// Creating a new post
currentUser.createPost("Hello World!", "image.jpg"); // Successful post creation
currentUser.createPost("", "video.mp4"); // Validation Error: Content cannot be empty.