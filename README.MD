# blog

## Initial setup

```bash
git clone $REPO
git submodule add git@github.com:faithinyous/hugo-PaperMod.git themes/PaperMod #using theme from karnwong
git submodule update --init --recursive
```

## Update theme

```bash
git submodule foreach git pull origin master
```

## Create a new post

```bash
./create-post.sh -n $TITLE -t $TAG

# with images
./create-post.sh -n $TITLE -t $TAG -i true
```

## Change google analytics

> config.yaml
> 
> googleAnalytics: $ID <-- change to your google tag ID

