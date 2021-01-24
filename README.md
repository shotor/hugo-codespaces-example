# hugo-codespaces-example

Example repository for Hugo and GitHub Codespaces.

Check out the [blog post](https://shotor.com/blog/build-a-hugo-static-site-in-your-browser-using-github-codespaces) for this repository.

Check out the demo at <https://pensive-sammet-17c943.netlify.app/>.

## Dependencies

- [Hugo](https://gohugo.io/)

## Usage

### Debug locally

```sh
hugo server -D
```

### Debug on codespaces

1. Open the `remote explorer` sidebar in Codespaces.
2. Forward port 1313
3. Right click on entry and copy the url

Run the server command with copied url

```sh
hugo server -D --baseUrl "https://{githubUrl}" --appendPort=false
```

### Build

```sh
hugo build
```

## License

MIT