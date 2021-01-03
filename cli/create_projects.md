# CLI - Creating Projects

Lets say we need two projects for our developers & dev-ops team
`development` & `production`

This would be as simple as;

`lxc project create development`

`lxc project create production`

Our server will now look something like this;

<img src="/assets/cli/imgs/1.png">

At time of writing a newly created project will have its own set of;

 - Instances
 - Images
 - Profiles
 - Storage Volumes

*You can read about theres terms [Here TODO](link)*

## Sharing Project Entities

Sometimes you may want to share certain entities amoung projects.

The most common use case that springs to mind is images, by sharing images
amoungst projects you can reduce the total storage used on each system.

If projects share entities, it shares entities with the `default` project.

*Sharing images is a security vulnreablity if you or your users publish
instances as images for re-use*

To share image between the `default` project & the `development` project you
would execute the command;

`lxc project set development features.images=false`

Assuming you have downloaded a few Ubuntu images in the `default` project, your
server will look something like the following & users in the `development`
project will be able to re-use the images without downloading them.

<img src="/assets/cli/imgs/2.png">
