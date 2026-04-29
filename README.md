Kenapa perlu volume untuk MySQL?
Supaya data database tidak hilang saat container dimatikan atau dihapus. Volume menyimpan data di harddisk laptop kita, bukan di dalam container yang sementara.

Apa fungsi depends_on?
Untuk mengatur urutan. WordPress tidak bisa jalan kalau MySQL belum siap, jadi depends_on memastikan MySQL nyala duluan sebelum WordPress.

Bagaimana cara WordPress container connect ke MySQL?
Menggunakan nama service-nya yaitu mysql sebagai hostname (karena mereka berada dalam satu network yang sama).

Apa keuntungan pakai Redis untuk WordPress?
Mempercepat loading website karena data yang sering diakses disimpan di RAM (Redis), jadi WordPress tidak perlu terus-terusan bertanya ke database MySQL.