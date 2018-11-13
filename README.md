# Steps to run hexo website
1. Install hexo cli.

```bash
$ npm install -g hexo-cli
```

1. Generate hexo website.

```bash
$ hexo init aikmeng-blog
```

1. Install dependencies to run website.
```bash
$ cd aikmeng-blog/
$ npm install
```

1. Run website
```bash
$ hexo server
```

1. Install deployment module
```bash
$ npm install hexo-deployer-git --save
```

1. Configure _config.yml
```yaml
# Deployment
## Docs: http://hexo.io/docs/deployment.html
deploy:
  type: git
  repo: git@github.com:aikmeng/aikmeng.github.io.git
  branch: master
```

1. Deployment
```bash
$ hexo clean
$ hexo deploy
```

1. Push to Git for version control
```bash
$ git init
$ git remote add origin git@github.com:aikmeng/aikmeng-blog.git
```

# Creating blog posts

1. Create new hexo post
``` bash
$ hexo new "My First Post"
```

2. Modify My-First-Post.md

1. Deployment
```bash
$ hexo clean
$ hexo deploy
```