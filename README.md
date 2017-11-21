# Free PMO
> *Tell our clients that we are managing our projects professionally.*

Free PMO (Project Management Office), software management project untuk *freelancer* dan agensi, dibangun dengan Framework **Laravel 5**.

### Daftar Isi
1. [Tentang Free PMO](#tentang)
2. [Tujuan](#tujuan)
3. [Cara Install](#cara-install)
    - [Spesifikasi yang Dibutuhkan](#spesifikasi-minimum-server)
    - [Tahap Install](#tahap-install)
4. [Developer dan Kontributor](#developer-dan-kontributor)
5. [Ingredients (Ramuan)](#ramuan)
6. [Lisensi](#license)
7. [Cara Berkontrobusi](#cara-berkontribusi)
8. [Screenshots](#screenshots)

<hr>

## Tentang

**Free PMO** adalah software yang bertujuan untuk mempermudah pengelolaan dan monitor project. Software ini cocok untuk *Freelancer* dan Agensi/*Software House*, atau perusahaan yang memiliki layanan *project based* kepada customernya.

**Free PMO** terdiri dari dua kata, yaitu *Free* dan *PMO*.
1. **Free** bisa jadi singkatan dari **Freelancer**, bisa juga **Free Software** (merdeka), dan tentunya **Free (gratis)**.
2. **PMO** singkatan dari ***Project Management Office***, ibarat kantor untuk pengelolaan project.

Fitur utama Free PMO adalah pengelolaan project dan transaksi pembayaran setiap project. Fitur-fitur lain software ini tertuang dalam file [konsep](CONCEPT.md){:target="_blank"}.

## Tujuan

Tujuan utama Free PMO adalah membantu pengelolaan data project dengan mudah dan profesional.

## Cara Install
Aplikasi ini dapat dipasang dalam server lokal (PC/Laptop) dan server online, dengan spesifikasi berikut :

#### Spesifikasi minimum server
1. PHP 7.0 (dan memenuhi [server requirement Laravel 5.5](https://laravel.com/docs/5.5#server-requirements){:target="_blank"}),
2. MySQL atau MariaDB,
3. SQlite (untuk automated testing).

#### Tahap Install

1. Clone Repo, pada terminal : `git clone https://github.com/nafiesl/free-pmo.git`
2. `$ cd free-pmo`
3. `$ composer install`
4. `$ cp .env.example .env`
5. `$ php artisan key:generate`
6. Buat database pada MySQL untuk aplikasi ini
7. Setting database pada file `.env`
8. `$ php artisan migrate`
9. `$ php artisan serve`
10. Kunjungi web : `http://localhost:8000/app-install`
11. Isi formulir installasi.
12. Selesai, Anda akan login sebagai admin.

<center>![Install Free PMO](public/screenshots/pmo-install-free-pmo.jpg)</center>


## Developer dan Kontributor

Project ini dikembangkan oleh [Nafies Luthfi](https://github.com/nafiesl) dan para [kontributor](https://github.com/nafiesl/free-pmo/graphs/contributors).

## Ramuan

Free PMO dibangun menggunakan [metode TDD](https://blog.nafies.id/laravel/testing-laravel-tentang-automated-testing){:target="_blank"} dengan bahan dan dukungan dari paket-paket berikut ini :

##### Dependencies
* [Framework Laravel](https://laravel.com/docs/5.5){:target="_blank"} (versi 5.2 s/d 5.5).
* [luthfi/formfield](https://github.com/nafiesl/FormField){:target="_blank"}, Wrapper Form dari [laravelcollective/html](https://github.com/laravelcollective/html){:target="_blank"} dengan Bootstrap 3.
* [riskihajar/terbilang](https://github.com/riskihajar/terbilang){:target="_blank"}, membuat angka terbilang (pada fitur cetak kuitansi) dan romawi.

##### Dev Dependencies

* [PHPUnit](https://github.com/sebastianbergmann/phpunit){:target="_blank"}, PHP testing framework.
* [laravel/browser-kit-testing](https://github.com/laravel/browser-kit-testing){:target="_blank"}, paket browserkit testing untuk Laravel ^5.4.
* [luthfi/simple-crud-generator](https://github.com/nafiesl/SimpleCrudGenerator){:target="_blank"}, CRUD generator berupa artisan command untuk mempercepat workflow TDD.
* [johnkary/phpunit-speedtrap](https://github.com/johnkary/phpunit-speedtrap){:target="_blank"}, pengecekan testing yang lambat (karena query atau proses yang kurang efektif).

## Lisensi

Project Free PMO merupakan software free dan open source di bawah [lisensi MIT](LICENSE).

## Cara Berkontribusi

Jika ingin berkontribusi terhadap project ini, baik untuk membuat *Issue*, usulan Fitur tambahan, *Pull Request*, maupun donasi, silakan melihat [panduan kontribusi](CONTRIBUTING.md){:target="_blank"}.

## Screenshots

#### Dashboard
![Free PMO Dashboard](public/screenshots/pmo-dashboard-01.jpg){:title="Free PMO Dashboard"}

#### Detail Project
![Free PMO Project Detail](public/screenshots/pmo-project-detail-01.jpg){:title="Free PMO Project Detail"}

#### List Job Project
![Free PMO Project Job List](public/screenshots/pmo-project-jobs-01.jpg){:title="Free PMO Project Job List"}

#### Detail Job Project
![Free PMO Job Tasks](public/screenshots/pmo-job-tasks-01.jpg){:title="Free PMO Job Tasks"}

#### Laporan Tahunan
![Free PMO Yearly Report](public/screenshots/pmo-yearly-report-01.jpg){:title="Free PMO Yearly Report"}

#### Automated Testing

```bash
$ vendor/bin/phpunit
```

<center>![Free PMO Testing](public/screenshots/pmo-testing-01.jpg){:title="Free PMO Automated Testing"}</center>