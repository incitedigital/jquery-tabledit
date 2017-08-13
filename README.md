# jQuery-Tabledit v1.2.5
Inline editor for HTML tables compatible with Bootstrap.

## Basic usage

1. Add the jQuery tabledit plugin after jQuery library.

```
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.2/jquery.min.js"></script>
<script src="jquery.tabledit.js"></script>
```


2. Create Bootstrap table with data

```
<table class="table table-hover" id="my-table">
    <thead>
        <tr>
            <th>Id</th>
            <th>Column 1</th>
            <th>Column 2</th>
            <th>Column 3</th>
            <th>Column 4</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1</td>
            <td>Data 1</td>
            <td>Data 2</td>
            <td>Data 3</td>
            <td>Data 4</td>
        </tr>
    </tbody>
</table>
```

3. Call the plugin on your existing table and specify the editable columns whatever you like.

```
$('#my-table').Tabledit({

    columns: {
      identifier: [0, 'id'],                    
      editable: [[1, 'col1'], [2, 'col1'], [3, 'col3'], [4, 'col4']]
    }

});
```


## Examples
Original example by _markcell_ you find on 
http://markcell.github.io/jquery-tabledit/#examples
 
**Readonly value in TD**

You set this in the editable array, if you want readonly leave the column out of the 'editable' array e.g.: Column 3 wouldn't be editable.

```
$('#my-table').Tabledit({

    columns: {
      identifier: [0, 'id'],                    
      editable: [[1, 'col1'], [2, 'col1'], [4, 'col4']]
    }

});
```

## Documentation
Original example by _markcell_ you find on
http://markcell.github.io/jquery-tabledit/#documentation

Full complete documentation by BluesatKV on 
https://bluesatkv.github.io/jquery-tabledit/#documentation


## Changelog
See CHANGELOG.md file.

