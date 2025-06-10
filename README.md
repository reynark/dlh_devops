# dlh_devops

--- Daha cok DOCKER
-- .workflows oldugu icin biraz gitops_stuff'a da yakin

Alistirmalardan biri:

On GitHub, create your workflow file.

Create a folder at the root of the repo: `.github/workflows`  ## bu folder'i yaratinca actions kismi aciliyo

Creating the .github/workflows directory in your repo tells GitHub where to look for GitHub Actions workflow files.

In this folder, create your actions file: `docker-image.yml`

On GitHub, prepare your environment variables:

- `DOCKER_USERNAME`
- `DOCKER_PASSWORD`

### Workflow Steps

1. Log in to your Docker Hub repository  
2. Build your image  
3. Push your image  
4. Log out
