## Demo
Install dependencies:

```console
$ make install
```

Prepare the demo:

```console
$ make demo
```

Run the server:

```console
$ make serve
```

Open your browser and go to [http://localhost:3000/](http://localhost:3000/)

## Props
| Name                      | Type        | Description                                                                                   |
| ---                       | ---         | ---                                                                                           |
| `pageCount`               | `Number`    | **Required.** The total number of pages.                                                      |
| `pageRangeDisplayed`      | `Number`    | **Required.** The range of pages displayed.                                                   |
| `marginPagesDisplayed`    | `Number`    | **Required.** The number of pages to display for margins.                                     |
| `previousLabel`           | `Node`      | Label for the `previous` button.                                                              |
| `nextLabel`               | `Node`      | Label for the `next` button.                                                                  |
| `breakLabel`              | `Node`      | Label for ellipsis.                                                                           |
| `breakClassName`          | `String`    | The classname on tag `li` of the ellipsis element.                                            |
| `onPageChange`            | `Function`  | The method to call when a page is clicked. Exposes the current page object as an argument.    |
| `initialPage`             | `Number`    | The initial page selected.                                                                    |
| `forcePage`               | `Number`    | To override selected page with parent prop.                                                   |
| `disableInitialCallback`  | `boolean`   | Disable `onPageChange` callback with initial page. Default: `false`                           |
| `containerClassName`      | `String`    | The classname of the pagination container.                                                    |
| `pageClassName`           | `String`    | The classname on tag `li` of each page element.                                               |
| `pageLinkClassName`       | `String`    | The classname on tag `a` of each page element.                                                |
| `activeClassName`         | `String`    | The classname for the active page.                                                            |
| `previousClassName`       | `String`    | The classname on tag `li` of the `previous` button.                                           |
| `nextClassName`           | `String`    | The classname on tag `li` of the `next` button.                                               |
| `previousLinkClassName`   | `String`    | The classname on tag `a` of the `previous` button.                                            |
| `nextLinkClassName`       | `String`    | The classname on tag `a` of the `next` button.                                                |
| `disabledClassName`       | `String`    | The classname for disabled `previous` and `next` buttons.                                     |
| `hrefBuilder`             | `Function`  | The method is called to generate the `href` attribute value on tag `a` of each page element.  |
| `extraAriaContext`        | `String`    | Extra context to add to the `aria-label` HTML attribute.                                      |
