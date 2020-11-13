
## setup

```shell
brew install hugo

hugo new site NEW_SITE_NAME
cd NEW_SITE_NAME
git init
git submodule add https://github.com/PATH_TO_THEME.git themes/THEME_NAME
echo 'theme = "THEME_NAME"' >> config.toml
```

## setup in prod

```shell
sudo mkdir ~/apps/blog
sudo chown bitnami ~/apps/blog
# edited /opt/bitnami/nginx/conf/bitnami/bitnami-apps-http.conf 
```

## new posts
```shell
hugo new posts/my-first-post.md
```

## pushing posts to production
```shell
# from base local directory:
hugo
./deploy
```

## operation
```shell
hugo server -D # run local server, with drafts
hugo # generate files, no drafts
```

## short codes example:
```go
{{< time.inline >}}{{ now }}{{< /time.inline >}}
```