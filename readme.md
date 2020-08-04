<p align="center">
  <img width="400" src="./image/demo.png">
  <h3 align="center">Bilibili-box</h3>
  <p align="center">Update a pinned gist to contain the latest videos of a user</p>
</p>

---

> 📌✨ For more pinned-gist projects like this one, check out: https://github.com/matchai/awesome-pinned-gists

## Setup

English | [中文](./readme.zh.md)

### Prep work

1. Create a new public GitHub Gist (https://gist.github.com/)
1. Create an access token with the `gist` scope and copy it. (https://github.com/settings/tokens/new)
1. Find UID in Bilibili personal space link (https://space.bilibili.com/37728693)


### Project setup

1. Fork this repo
1. Edit the [environment variables](https://github.com/KeJunMao/bilibili-box/blob/master/.github/workflows/main.yml#L27-L28) in `.github/workflows/schedule.yml`:

   - **UID:** The user handle of the bilibili account.
   - **GIST_ID:** The ID portion from your gist url: `https://gist.github.com/matchai/`**`6d5f84419863089a167387da62dd7081`**.

1. Go to the repo **Settings > Secrets**
1. Add the following environment variables:
   - **GH_TOKEN:** The GitHub access token generated above.
