# react-datatable
React datatable helper
Sample Data
```javascript
    this.state = {
        columns: [
            {key: 'date', title: "Date"},
            {key: 'in1', title: "Time-In (Morning)"},
            {key: 'out1', title: "Time-Out"},
            {key: 'in2', title: "Time-In (Afternoon)"},
            {key: 'out2', title: "Time-Out"},
            {key: 'totalHours', title: "Total Hrs", },
            {key:'action', title:'action', cell: (row) => this.actions(row) }
        ],
        data:[], 
        recordsTotal: 0 
    } 
```
Initialization
```typescript
    <DatatableHelper 
        columns={this.state.columns}
        data={this.state.data}
        onChangePage={(page) => { console.log(page) }} 
    />  
```
