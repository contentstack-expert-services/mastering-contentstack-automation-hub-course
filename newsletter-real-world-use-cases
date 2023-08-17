const posts = input.blog;

const generatePostHTML = (post) => {
  return `
    <div class="post">
      <h2 class="post-title">${post.title}</h2>
      <p class="post-excerpt">${post.content}</p>
      <a class="cta-button" href="#">Read More</a>
    </div>
  `;
};

const generateHTMLTemplate = (posts) => {
  const postContents = posts.map(generatePostHTML).join('');
  
  return `
    <!DOCTYPE html>
    <html>
    <head>
      <meta charset="UTF-8">
      <title>Your Blog Newsletter</title>
      <style>
        /* Your CSS styles here */
      </style>
    </head>
    <body>
      <div class="container">
        <div class="header">
          <h1>Your Blog Newsletter</h1>
        </div>
        <div class="content" id="content">
          ${postContents}
        </div>
        <div class="footer">
          <p>&copy; 2023 Your Blog. All rights reserved.</p>
        </div>
      </div>
    </body>
    </html>
  `;
};

const htmlTemplate = generateHTMLTemplate(posts);

// Output to console
return htmlTemplate;

// Alternatively, you can save the content to a file manually, if needed
// const outputPath = 'output.html';
// fs.writeFileSync(outputPath, htmlTemplate);
// console.log(`HTML template generated and saved as ${outputPath}`);
