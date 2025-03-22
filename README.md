# LaTeX Docker Builder

Docker container that contains a LaTeX environment to build LaTeX documents.

## Usage

```bash
docker run --rm -i --user="$(id -u):$(id -g)" --net=none -v "$PWD":/data yawnwest/latexbuilder:latest lualatex main.tex

# running lualatex twice
docker run --rm -i --user="$(id -u):$(id -g)" --net=none -v "$PWD":/data yawnwest/latexbuilder:latest /bin/sh -c "lualatex main.tex && lualatex main.tex"
```

## License

[MIT](https://choosealicense.com/licenses/mit/)
