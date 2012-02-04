## Distributed City Documentation Project

#### Documentation System Based on Code from the *awesome* Nodejitsu
https://github.com/nodejitsu/docs

#### The source files in this project are used to generate the website:
http://distributedcity.github.com/

## Usage

### Browse Online:
http://distributedcity.github.com/

### Browse Localy:

#### Checkout and Generate the docs

    node bin/docs generate
    
#### To start the docs server

    node bin/docs serve

### Contribute:

*Fork, make changes, additions, submissions, and give us a PULL request.*

### To add an article:

- make a directory in `topics` for your article: `mkdir articles/how-to-make-an-article` (use only letters and dashes)
- next write your article: `vim articles/how-to-make-an-article/content.md`
- create a metadata with this data: `vim articles/how-to-make-an-article/page.json`

**metadata.json**

```javascript
{
  "title":"What is npm?",
  "date": "Fri Aug 26 2011 03:08:50 GMT-0700 (PST)",
  "tags": ["npm", "modules"],
  "author": "Nico Reed",
  "difficulty": 1
}
```


### Directory Structure

    topics/
        article-name/ //url version
            page.json
            content.md //file with the real article
            assets/
                ...
        ...

### Metadata Format

```javascript
{
  "title":"What is npm?",
  "date": "Fri Aug 26 2011 03:08:50 GMT-0700 (PST)",
  "tags": ["npm", "modules"],
  "author": "Nico Reed",
  "difficulty": 1
}
```
