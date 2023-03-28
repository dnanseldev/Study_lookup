# ngFor only works in lists or collections (arrays) not in single object
# Including an index to ngFor loop angular allows you indexing the iteration ex:

<tr *ngFor="let item of items"; let i = index>
  <td>{{i}}</td>
  <td>{{item.property}}</td>
</tr>
