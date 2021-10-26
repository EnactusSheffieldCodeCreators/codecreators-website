# Code Creators Website

## Install notes

Install rvm
install ruby version 3.0.2
`gem install bundler jekyll`
`bundle install`
`bundle exec jekyll serve`

## Editing The Site

### Team members

First how to add images, if you do not have one for someone then simply skip this step. Add images to the folder `assets/images/team/original-photos` before rescaling them to 512x512 pixels and exporting that image into the folder `assets/images/team/reformatted`. This isn't highly necessary but it helps with keeping the site fast.

Next to add the team member inside the header section to `index.md` there is a bit of YAML that looks similar to this:

```YAML
team_feature_row:
  - image_path: assets/images/team/reformatted/<NAME>.webp
    alt: "<NAME>"
    title: "<NAME>"
    excerpt: "<ROLE>"
  - image_path: assets/images/team/reformatted/<NAME>.webp
    alt: "<NAME>"
    title: "<NAME>"
    excerpt: "<ROLE>"
```

From here copy the format of one of the entries and add the image path and details for the new team member. If you are not using an image then use `assets/images/team/placeholder.svg` as the image.
