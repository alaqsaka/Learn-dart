# Learn-dart

Coding Language: Dart
Technologies: IntelliJ IDEA & Windows 

## 9 Januari 2021
1. Break and Continue
2. Switch and case 
3. Collections(list, set, and map)

### LIST
```
// Cara penulisan list:
List<int> listAngkaGanjil = [1,3,5,7,9];

// bisa ditulis tanpa tipe datanya 
// var listAngkaGanjil = [1,3,5,7,9];
var kata = ['Dart', 'Hujan', 'Kopi'];

// kalo ga ditulis => dinamis (menyimpan semua tipe data)

print('Indexing dalam bahasa Dart juga dimulai dari 0 ^^');

// Cara mencetak elemen-elemen yang ada di list: 

// Cara Satu (menggunakan for loop):

for(int x; x < listAngkaGanjil.length; x++){
  print(listAngkaGanjil[i]);
}

// cara kedua (menggunakan forEach() => lambda / anonymus function

kata.forEach((s) => print (s));


// Manipulasi data di LIST
listAngkaGanjil.add(11);
listAngkaGanjil.insert(0, -1); 
listAngkaGanjil.remove(3) // Menghapus list dengan nilai 3
listAngkaGanjil.removeAt(1); // Menghapus list pada index ke-1
listAngkaGanjil.removeLast(); // Menghapus data list terakhir
listAngkaGanjil.removeRange(1,3); //  // Menghapus list mulai index ke-1 sampai ke-3 (indeks 3 masih dipertahankan)
```

### SET
```
// DEKLARASI SET
var angka = {1,2,3};
Set<int> angkaGenap = newt Set.from([2,3,4,5,6,7]);

print(angkaGenap) // mencetak angka yang beda saja

// MANIPULASI SET
angka.remove(3); // menghaous angka yang diinginkan
angka.add(9); // menambahkan data ke dalam set 
angka.addAll({101,102,103});

print(angka.elementAt(0)); // menampilkan data pada index tertentu

// union and intersection 
var union = angka.union(angkaGenap);
var intersection = angka.intersection(angkaGenap);
```

### MAP
```
key-value
key = apel
  value = merah
  var buah = {
  'apel': 'merah'
  };
  
  print(buah['apel']); 
  // output: merah
  
  // menampilkan seluruh keys 
  var buahKeys = buah.keys;
  // menampilkan nilai
  var buahValues = buah.values;
  // menambahkan value baru
  buah['mangga'] = 'ijo';
  
```


## 12 Januari 2021
1. Mixins 
-> menggunakan kembali kode kelas dalam banyak hirarki kelas.
Cara mendefiniskan mixin sama seperti class
```
mixin berjalan{
void jalan(){
  print("Saya jalan");
    }
}
```
