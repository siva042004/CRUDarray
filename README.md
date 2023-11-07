# CRUD-using-Array-of-Object
```
let dataArray = [];
function addData(name, age, city) {
  const newData = { name, age, city };
  dataArray.push(newData);
  console.log('Added:', newData);
}

function editData(index, name, age, city) {
  if (index >= 0 && index < dataArray.length) {
    dataArray[index] = { name, age, city };
    console.log('Edited:', dataArray[index]);
  } else {
    console.log('Invalid index for editing.');
  }
}

function deleteData(index) {
  if (index >= 0 && index < dataArray.length) {
    const deletedData = dataArray.splice(index, 1)[0];
    console.log('Deleted:', deletedData);
  } else {
    console.log('Invalid index for deletion.');
  }
}

function showData() {
  console.log('Current Data:');
  dataArray.forEach((data, index) => {
    console.log(`[${index}]`, data);
  });
}

addData('John Doe', 25, 'New York');
addData('Jane Doe', 30, 'Los Angeles');
showData();

editData(0, 'John Updated', 26, 'New York');
showData();

deleteData(1);
showData();
```
# output
![image](https://github.com/21002624/CRUD-using-Array-of-Object/assets/113762183/ec634d44-c550-4a8d-9684-c590a4b579a8)

