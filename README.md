# Steps to run hexo website
Install hexo cli.

```bash
$ npm install -g hexo-cli
```

Generate hexo website.

```bash
$ hexo init aikmeng-blog
```

Install dependencies to run website.
```bash
$ cd aikmeng-blog/
$ npm install
```

Run website
```bash
$ hexo server
```

Install deployment module
```bash
$ npm install hexo-deployer-git --save
```

Configure _config.yml
```yaml
# Deployment
## Docs: http://hexo.io/docs/deployment.html
deploy:
  type: git
  repo: git@github.com:aikmeng/aikmeng.github.io.git
  branch: master
```

Deployment
```bash
$ hexo clean
$ hexo deploy
```

Push to Git for version control
```bash
$ git init
$ git remote add origin git@github.com:aikmeng/aikmeng-blog.git
```

# Creating blog posts

Create new hexo post
``` bash
$ hexo new "My First Post"
```

Modify My-First-Post.md
```markdown
title: My First Post
date: 2018-11-14 03:22:01
tags:

Hello World!
```

Deploy blog post
```bash
$ hexo clean
$ hexo deploy
```