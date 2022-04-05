## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/VLDG1l/_linkGit/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/VLDG1l/_linkGit/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.


<script>
  document.cookie = "session=test GDPR"; 
  document.cookie = "favorite_task=collect Data"; 
  document.cookie = "name=oeschger; SameSite=None; Secure";
  document.cookie = "favorite_food=tripe; SameSite=None; Secure";
  document.cookie = "reader=1; SameSite=None; Secure";
  
  function alertCookie() {
    alert(document.cookie); 
  } 
  
  function showCookies() {
    const output = document.getElementById('cookies')
    output.textContent = '> ' + document.cookie
  }
  
  function checkACookieExists() {
    if (document.cookie.split(';').some((item) => item.trim().startsWith('reader='))) {
      const output = document.getElementById('a-cookie-existence')
      output.textContent = '> The cookie "reader" exists'
    }
  }
  
  function checkCookieHasASpecificValue() {
    if (document.cookie.split(';').some((item) => item.includes('reader=1'))) {
      const output = document.getElementById('a-specific-value-of-the-cookie')
      output.textContent = '> The cookie "reader" has a value of "1"'
    }
  }

  function clearASpecificValueOfTheCookie() {
    const output = document.getElementById('a-specific-value-of-the-cookie')
    output.textContent = ''
  }
  
  function clearOutputCookies() {
    const output = document.getElementById('cookies')
    output.textContent = ''
  }
</script>

<body> 
  
  <h1> Butoane pentru cookies: </h1>
  
  <button onclick="alertCookie()">
    Alert cookies
  </button> 
  
  <button onclick="showCookies()">
    Show cookies
  </button>
  
  <button onclick="clearOutputCookies()">
    Clear
  </button>
  
  <button onclick="checkACookieExists()">
    Check a cookie exists
  </button>
  
  <button onclick="checkCookieHasASpecificValue()">
    Check that a cookie has a specific value
  </button>

  <button onclick="clearASpecificValueOfTheCookie()">
    Clear a specific cookie
  </button>
  
  <div>
    <p> All coockies: </p>
    <code id="cookies"></code>
  </div>  
  
   <div>
    <p> A cookie existance: </p>
    <code id="a-cookie-existence"></code>
  </div>  
  
  <div>
    <p> Specific cookie: </p>
    <code id="a-specific-value-of-the-cookie"></code>
  </div>  
  
</body>
