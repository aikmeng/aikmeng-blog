# Hexo Web Site Configuration
1. Generate hexo website.

```console
$ hexo init aikmeng-blog
```

2. Install dependencies to run website.
```console
$ cd aikmeng-blog/
$ npm install
```

3. Run website
```console
$ hexo server
```

4. Install deployment module
```console
$ npm install hexo-deployer-git --save
```

5. Configure _config.yml
```yaml
# Deployment
## Docs: http://hexo.io/docs/deployment.html
deploy:
  type: git
  repo: git@github.com:aikmeng/aikmeng.github.io.git
  branch: master
```

6. Deployment
```console
$ hexo clean
$ hexo deploy
```

7. Push to Git for version control
```console
$ git init
$ git remote add origin git@github.com:aikmeng/aikmeng-blog.git
```