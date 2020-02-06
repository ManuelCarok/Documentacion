[Volver](../../README.md)

![Banner](../../img/banners/gitbook.jpg)

# GitBook

> ⚠️ leer documentación official [documentación](https://www.npmjs.com/package/gitbook)

## Cómo usarlo:

GitBook se puede instalar desde NPM usando:

```bash
$ npm install gitbook-cli -g
```

Cree los directorios y archivos para un libro desde su archivo **SUMMMARY.md** (si existe) usando

```bash
$ gitbook init
```

Puede servir un repositorio como libro usando:

```bash
$ gitbook serve
```

O simplemente construya el sitio web estático usando:

```bash
$ gitbook build
```

## Formatos de salida

GitBook puede generar su libro en los siguientes formatos:

* **Sitio web estático:** este es el formato predeterminado. Genera un sitio web estático interactivo completo que puede, por ejemplo, alojarse en páginas GitHub.
  
* **eBook:** necesita tener instalado ebook-convert. Puede especificar el nombre de archivo del libro electrónico como segundo argumento; de lo contrario, se utilizará el libro.
  
    * Genere un PDF usando: `gitbook pdf ./myrepo ./mybook.pdf`
    * Genere un ePub usando: `gitbook epub ./myrepo ./mybook.epub`
    * Genere un MOBI usando: `gitbook mobi ./myrepo ./mybook.mobi`
    * 
* **JSON:** este formato se utiliza para depurar o extraer metadatos de un libro. Genere este formato usando: `gitbook build ./myrepo --format = json`