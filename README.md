# pure-css-modal
> simple pure css modal, just for fun

```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>pure css modal</title>
      <style>
      body {
        padding: 8px;
      }
      label {
        display: inline-block;
        color: #fff;
        padding: 10px 15px;
        background-color: #3c8dbc;
        border-color: #367fa9;
        border-radius: 4px;
        cursor: pointer;
      }
      .checker:checked + .modal {
        display: flex;
      }
      .modal {
        display: none;
        justify-content: center;
        align-items: center;
        position: fixed;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        text-align: center;
        background-color: rgba(0,0,0,.4);
      }
      .modal-body {
        width: 200px;
        background-color: #fff;
        border-radius: 4px;
        padding: 15px;
      }
      .modal-content {
        padding: 15px;
      }
      .modal-footer {
        overflow: hidden;
      }
      </style>
    </head>
    <body>
      <label for="o">open</label>
      <input class="checker" type="checkbox" id="o" hidden>
      <div class="modal">
        <div class="modal-body">
          <div class="modal-content">Aloha!</div>
          <div class="modal-footer">
            <label for="o">close</label>
          </div>
        </div>
      </div>
    </body>
  </html>
```
