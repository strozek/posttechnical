
# setup

brew install hugo

hugo new site NEW_SITE_NAME
cd NEW_SITE_NAME
git init
git submodule add https://github.com/PATH_TO_THEME.git themes/THEME_NAME
echo 'theme = "THEME_NAME"' >> config.toml


# in prod

sudo mkdir ~/apps/blog
sudo chown bitnami ~/apps/blog

# edited /opt/bitnami/nginx/conf/bitnami/bitnami-apps-http.conf 

# to push to prod, from base local directory:
./deploy


# new post

hugo new posts/my-first-post.md


# operation

hugo server -D # run local server, with drafts
hugo # generate files, no drafts


# short codes example:

{{< time.inline >}}{{ now }}{{< /time.inline >}}