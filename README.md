# Host Hugo on Github Pages with Custom Domain

1. Rename publish directory and set base url in [`config.toml`](/config.toml)

    ```toml
    baseURL = "https://lakto.pupraki.com/"
    ...
    publishDir = "docs"
    ```

2. Set source to `/docs` and set custom domain to `lakto.pupraki.com` in https://github.com/puplakto/blog/settings/pages

3. Add a CNAME record in DNS, pointing `lakto.pupraki.com` to `puplakto.github.io`

4. Run `hugo` to generate static files and push the repo, wait for Github Action workflow to complete.