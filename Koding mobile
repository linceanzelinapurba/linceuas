import 'package:flutter/material.dart';

void main() => runApp(App04());

class App04 memperluas StatelessWidget {
  Pembuatan widget (konteks BuildContext) {
    kembalikan MaterialApp(
      rute: {
        "Data": (konteks) => LinceAnzelinaPurbaDataTable(),
        "Lupa": (konteks) => LupaPass(),
        "aritmatika": (konteks) => Aritmatika(),
      },
      judul: 'FORM LOGIN',
      rumah: Perancah (
        appBar: AppBar(
          judul: Teks('UAS-Lince Anzelina Purba (6SIA1)'),
        ),
        isi: Halaman Masuk(),
      ),
    );
  }
}

class LoginPage memperluas StatefulWidget {
  _LoginPageState createState() => baru _LoginPageState();
}

class _LoginPageState memperluas Status<LoginPage> {
  
  akhir myNirm = TextEditingController();
  
  Tali nirma;

  masuk () {
    nirm = myNirm.text;
    if (nirm == '2018020546' ) {
      Navigator.pushNamed(konteks, "Data");
    } lain {
      Navigator.pushNamed(konteks, "Lupa");
    }
  }

  Pembuatan widget (konteks BuildContext) {

    id akhir = TextFormField(
      keyboardType: TextInputType.emailAddress,
      fokus otomatis: salah,
      pengontrol: myNirm,
      dekorasi: InputDecoration(
        ikon: Ikon (
        Ikon.orang,
        warna: Colors.blue
        ),
        petunjukTeks: 'NIRM',
        contentPadding: EdgeInsets.fromLTRB (20.0, 10.0, 20.0, 10.0),
        perbatasan: OutlineInputBorder(borderRadius: BorderRadius.circular(32.0)),
      ),
    );


    tombol login terakhir = Padding(
      padding: EdgeInsets.symmetric(vertikal: 16.0),
      anak: Bahan (
        borderRadius: BorderRadius.circular(30.0),
        shadowColor: Colors.lightBlueAccent.shade100,
        ketinggian: 5.0,
        anak: MaterialButton (
          minLebar: 200.0,
          tinggi: 42.0,
          onPressed:onLogin,
            // () {Navigator.pushNamed(context, "myApp");},
          warna: Colors.lightBlueAccent,
          anak: Text('Masuk', style: TextStyle(color: Colors.white)),
        ),
      ),
    );

    kembali Perancah (
      backgroundColor: Warna.putih,
      tubuh: Pusat (
        anak: ListView(
          shrinkWrap: benar,
          padding: EdgeInsets.only (kiri: 24.0, kanan: 24.0),
          anak-anak: <Widget>[
   
            SizedBox (tinggi: 48.0),
            Indo,
            SizedBox (tinggi: 8.0),
            tombol masuk,
          ],
        ),
      ),
    );
  }
}
 class LupaPass memperluas StatelessWidget {
  Pembuatan widget (konteks BuildContext) {
    kembali Perancah (
        appBar: AppBar(
          judul: Teks('Lupa NIRM'),
        ),
        //tubuh
        body: Text("Nirm Yang Anda Masukkan Salah"));
  }
}
class LinceAnzelinaPurbaDataTable memperluas StatefulWidget {
  _LinceAnzelinaPurbaDataTableState createState() => _LinceAnzelinaPurbaDataTableState();
}

class _LinceAnzelinaPurbaDataTableState memperluas State<LinceAnzelinaPurbaDataTable> {
  Daftar<DataMahasiswa> barang;

  batal initState() {
    super.initState();
    barang = DataMahasiswa.getDataBarang();
  }

  Pembuatan widget (konteks BuildContext) {
    kembali Perancah (
      appBar: AppBar(
        judul: Teks('Lince Anzelina Purba - 6SIA1'),
      ),
      tubuh: ListView(anak-anak: <Widget>[
        Pusat(
            anak: Text('Data Mahasiswa',
                style: TextStyle(fontSize: 20, fontWeight: FontWeight.bold))),
        Tabel data(
          kolom: [
            Kolom Data(label: Teks('')),
            Kolom Data(label: Teks('')),
          ],
          baris: barang
              .peta(
                (barang) => DataRow(sel: [
                  Sel Data(Teks(barang.id)),
                  DataCell(Teks(barang.namabarang)),
                ]),
              )
              .toList(),
        ),
        Lapisan(
      padding: EdgeInsets.symmetric(vertikal: 16.0),
      anak: Bahan (
        borderRadius: BorderRadius.circular(30.0),
        shadowColor: Colors.lightBlueAccent.shade100,
        ketinggian: 5.0,
        anak: MaterialButton (
          minLebar: 200.0,
          tinggi: 42.0,
          Ditekan:
            () {Navigator.pushNamed(konteks, "aritmatika");},
          warna: Colors.lightBlueAccent,
          anak: Text('Program Aritmatika', style: TextStyle(color: Colors.white)),
        ),
      ),
    ),
      ]),
    );
  }
}

kelas DataMahasiswa {
  //Atribut
  nomor string;
  String nama barang;
  

  //Konstruktor
  DataMahasiswa({this.id, this.namabarang});

  //Daftar Data
  static Daftar<DataMahasiswa> getDataBarang() {
    kembalikan <DataMahasiswa>[
      DataMahasiswa(
          id: "Nama", namabarang: "Lince Anzelina Purba", ),
      DataMahasiswa(
          id: "Jenis Kelamin", namabarang: "perempuan", ),
      DataMahasiswa(id: "Alamat", namabarang: "Jl.Jamin Ginting,Gang Medan area No.15", ),
      DataMahasiswa(
          id: "Jurusan", namabarang: "Sistem Informasi",),

    ];
    
  }
}
class Aritmatika extends StatefulWidget {
  _AritmatikaState createState() => new _AritmatikaState();
}

class _AritmatikaState meluas State<Aritmatika> {
  
 akhir xNama = TextEditingController();
  akhir xJumlah = TextEditingController();
final xHarga = TextEditingController();
  
  hasil string;

  diHitung() {
    keadaan set(() {
      var jumlah= int.parse(xJumlah.text) * int.parse(xHarga.text);
      hasil = "$jumlah";
    });
  }

  Pembuatan widget (konteks BuildContext) {

    id akhir = TextFormField(
      fokus otomatis: salah,
      pengontrol: xNama,
      dekorasi: InputDecoration(
        hintText: 'Nama',
        contentPadding: EdgeInsets.fromLTRB (20.0, 10.0, 20.0, 10.0),
        perbatasan: OutlineInputBorder(borderRadius: BorderRadius.circular(32.0)),
      ),
    );
    
    jmlah terakhir = TextFormField(
      fokus otomatis: salah,
      pengontrol: xJumlah,
      dekorasi: InputDecoration(
        petunjukTeks: 'Jumlah',
        contentPadding: EdgeInsets.fromLTRB (20.0, 10.0, 20.0, 10.0),
        perbatasan: OutlineInputBorder(borderRadius: BorderRadius.circular(32.0)),
      ),
    );

    hrga terakhir = TextFormField(
      keyboardType: TextInputType.emailAddress,
      fokus otomatis: salah,
      pengontrol: xHarga,
      dekorasi: InputDecoration(
        hintText: 'Harga',
        contentPadding: EdgeInsets.fromLTRB (20.0, 10.0, 20.0, 10.0),
        perbatasan: OutlineInputBorder(borderRadius: BorderRadius.circular(32.0)),
      ),
    );



    tombol login terakhir = Padding(
      padding: EdgeInsets.symmetric(vertikal: 16.0),
      anak: Bahan (
        borderRadius: BorderRadius.circular(30.0),
        shadowColor: Colors.lightBlueAccent.shade100,
        ketinggian: 5.0,
        anak: MaterialButton (
          minLebar: 200.0,
          tinggi: 42.0,
          onPressed:onHitung,
            // () {Navigator.pushNamed(context, "myApp");},
          warna: Colors.lightBlueAccent,
          anak: Text('Hitung', style: TextStyle(color: Colors.white)),
        ),
      ),
    );

    kembali Perancah (
      backgroundColor: Warna.putih,
      tubuh: Pusat (
        anak: ListView(
          shrinkWrap: benar,
          padding: EdgeInsets.only (kiri: 24.0, kanan: 24.0),
          anak-anak: <Widget>[
   
            SizedBox (tinggi: 48.0),
            Indo,
            SizedBox (tinggi: 48.0),
            jmlah,
            SizedBox (tinggi: 48.0),
            hrga,
            SizedBox (tinggi: 8.0),
            tombol masuk,
          ],
        ),
      ),
    );
  }
}
