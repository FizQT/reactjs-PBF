# reactjs-PBF
{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyPwhM3WcX65jwIdOTCiH5Bo",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/FizQT/reactjs-PBF/blob/master/README_md.ipynb\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "**APA ITU REST PARAMETER?**"
      ],
      "metadata": {
        "id": "0bMbteOz2O65"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Rest parameter adalah sebuah fitur pada JavaScript yang memungkinkan sebuah fungsi untuk menerima sejumlah argumen yang tidak terbatas dalam bentuk array. Dalam fungsi, rest parameter didefinisikan menggunakan tanda tiga titik (ellipsis) di depan nama parameter, seperti contoh berikut:"
      ],
      "metadata": {
        "id": "aiA0p1y_2hJF"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "function jumlahkan(...angka) {\n",
        "  let hasil = 0;\n",
        "  for (let i = 0; i < angka.length; i++) {\n",
        "    hasil += angka[i];\n",
        "  }\n",
        "  return hasil;\n",
        "}\n",
        "\n",
        "console.log(jumlahkan(1, 2, 3, 4, 5)); // Output: 15"
      ],
      "metadata": {
        "id": "J6SolgV62s9D"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Dalam contoh di atas, rest parameter **...angka** memungkinkan fungsi **jumlahkan** menerima argumen sebanyak apapun dan memasukkannya ke dalam array **angka**. Kemudian, array **angka** tersebut diiterasi dan dijumlahkan, lalu hasilnya dikembalikan dari fungsi tersebut. Dengan rest parameter, kita tidak perlu menentukan berapa banyak argumen yang akan diterima oleh sebuah fungsi, sehingga fungsi tersebut lebih fleksibel dan mudah digunakan."
      ],
      "metadata": {
        "id": "bqhWDvCs2nfq"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "**CARA MEMBUAT REST PARAMETER**"
      ],
      "metadata": {
        "id": "8Oa0mEs62z9x"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Untuk membuat rest parameter pada sebuah fungsi JavaScript, Anda hanya perlu menambahkan tanda tiga titik (ellipsis) di depan nama parameter pada definisi fungsi. Berikut adalah contoh sederhana cara membuat rest parameter:"
      ],
      "metadata": {
        "id": "lzX5VNZ528aQ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "function contohRestParameter(...argumen) {\n",
        "  console.log(argumen);\n",
        "}\n",
        "\n",
        "contohRestParameter('satu', 'dua', 'tiga');\n",
        "// Output: [\"satu\", \"dua\", \"tiga\"]"
      ],
      "metadata": {
        "id": "VDordlAo3GX9"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Dalam contoh di atas, fungsi **contohRestParameter** memiliki parameter **...argumen** yang berfungsi sebagai rest parameter. Ketika fungsi tersebut dipanggil dengan tiga argumen, argumen-argumen tersebut akan dikumpulkan ke dalam sebuah array dengan nama **argumen**. Kemudian array **argumen** tersebut dicetak pada konsol menggunakan **console.log()**."
      ],
      "metadata": {
        "id": "R3iogdnI3LvV"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Kita dapat mengakses elemen-elemen pada rest parameter menggunakan metode yang sama seperti mengakses elemen-elemen pada sebuah array, seperti contoh di bawah ini:"
      ],
      "metadata": {
        "id": "LGCrMTWD3WXJ"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "function jumlahkan(...angka) {\n",
        "  let hasil = 0;\n",
        "  for (let i = 0; i < angka.length; i++) {\n",
        "    hasil += angka[i];\n",
        "  }\n",
        "  return hasil;\n",
        "}\n",
        "\n",
        "console.log(jumlahkan(1, 2, 3, 4, 5)); // Output: 15"
      ],
      "metadata": {
        "id": "R9Db7iK13Si_"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Dalam contoh di atas, rest parameter **...angka** berfungsi untuk mengumpulkan argumen-argumen yang diterima oleh fungsi **jumlahkan** ke dalam sebuah array yang dinamakan **angka**. Kemudian, array **angka** tersebut diiterasi dan dijumlahkan menggunakan perulangan **for**. Akhirnya, hasil penjumlahan dikembalikan dari fungsi tersebut."
      ],
      "metadata": {
        "id": "YoRHqFQu3cV9"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "**KAPAN MENGGUNAKAN REST PARAMETER?**"
      ],
      "metadata": {
        "id": "xSQ1BUyg7KBs"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Rest parameter pada JavaScript sangat berguna ketika kita ingin membuat sebuah fungsi yang dapat menerima sejumlah argumen dengan jumlah yang tidak pasti. Dengan menggunakan rest parameter, kita dapat mengumpulkan argumen-argumen tersebut ke dalam sebuah array yang dapat diakses di dalam fungsi. Beberapa contoh kasus penggunaan rest parameter pada fungsi adalah:"
      ],
      "metadata": {
        "id": "0ylXTuLv7N7c"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "\n",
        "\n",
        "1.   Menghitung jumlah argumen pada fungsi\n",
        "\n"
      ],
      "metadata": {
        "id": "2NOJB_vM7Rm3"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Rest parameter dapat digunakan untuk menghitung jumlah argumen yang diterima oleh sebuah fungsi. Kita dapat mengakses panjang array rest parameter untuk mengetahui jumlah argumen yang diterima oleh fungsi.<BR>Contoh:"
      ],
      "metadata": {
        "id": "9SoCxDI97dlB"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "function hitungJumlahArgumen(...args) {\n",
        "  console.log(`Jumlah argumen yang diterima: ${args.length}`);\n",
        "}\n",
        "\n",
        "hitungJumlahArgumen(); // Output: Jumlah argumen yang diterima: 0\n",
        "hitungJumlahArgumen(1, 2, 3); // Output: Jumlah argumen yang diterima: 3\n",
        "hitungJumlahArgumen('satu', 'dua', 'tiga', 'empat'); // Output: Jumlah argumen yang diterima: 4"
      ],
      "metadata": {
        "id": "Hv5Jl_Xq7i4H"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "2. Menggabungkan beberapa array"
      ],
      "metadata": {
        "id": "4LvyaDNn7mkl"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Rest parameter dapat digunakan untuk mengumpulkan beberapa array ke dalam sebuah array baru.<br>Contoh:"
      ],
      "metadata": {
        "id": "eeWx_DTp7tCN"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "function gabungkanArray(...arrays) {\n",
        "  let hasil = [];\n",
        "  for (let i = 0; i < arrays.length; i++) {\n",
        "    hasil = hasil.concat(arrays[i]);\n",
        "  }\n",
        "  return hasil;\n",
        "}\n",
        "\n",
        "const arr1 = [1, 2, 3];\n",
        "const arr2 = [4, 5, 6];\n",
        "const arr3 = [7, 8, 9];\n",
        "\n",
        "console.log(gabungkanArray(arr1, arr2, arr3));\n",
        "// Output: [1, 2, 3, 4, 5, 6, 7, 8, 9]"
      ],
      "metadata": {
        "id": "Ct97tdYx70pC"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "3. Menghitung total dari sejumlah angka"
      ],
      "metadata": {
        "id": "JTaHL92o73nM"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Rest parameter dapat digunakan untuk mengumpulkan sejumlah angka yang akan dijumlahkan."
      ],
      "metadata": {
        "id": "Y5bShc0I7-rH"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "function jumlahkanAngka(...angka) {\n",
        "  let hasil = 0;\n",
        "  for (let i = 0; i < angka.length; i++) {\n",
        "    hasil += angka[i];\n",
        "  }\n",
        "  return hasil;\n",
        "}\n",
        "\n",
        "console.log(jumlahkanAngka(1, 2, 3, 4, 5)); // Output: 15"
      ],
      "metadata": {
        "id": "_3fcUYtA8BJ_"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "**PERBEDAAN REST PARAMETER DENGAN SPREAD OPERATOR**"
      ],
      "metadata": {
        "id": "lDRk0_Wj8EHE"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Spread operator dan rest parameter merupakan dua fitur yang saling berhubungan pada JavaScript. Namun, keduanya memiliki perbedaan dalam cara penggunaannya."
      ],
      "metadata": {
        "id": "7NFvLnGX8NOV"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Spread operator ditandai dengan tiga titik (ellipsis) yang digunakan untuk \"menyebar\" elemen-elemen dari sebuah array atau objek ke tempat lain. Berikut adalah contoh penggunaan spread operator pada array:"
      ],
      "metadata": {
        "id": "wOyegh8U9BNt"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "const arr1 = [1, 2, 3];\n",
        "const arr2 = [4, 5, 6];\n",
        "\n",
        "const arr3 = [...arr1, ...arr2];\n",
        "\n",
        "console.log(arr3); // Output: [1, 2, 3, 4, 5, 6]"
      ],
      "metadata": {
        "id": "Nz_xLn_g8T4v"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Dalam contoh di atas, spread operator **'...'** digunakan untuk menggabungkan elemen-elemen dari dua buah array (**arr1** dan **arr2**) ke dalam sebuah array baru yang dinamakan **arr3**. Spread operator memungkinkan kita untuk menyebar elemen-elemen dari sebuah array atau objek ke tempat lain, seperti dalam contoh di atas."
      ],
      "metadata": {
        "id": "mXf2GP-f8aUd"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Sementara itu, rest parameter juga menggunakan tanda tiga titik, tetapi pada posisi yang berbeda. Rest parameter digunakan pada definisi sebuah fungsi dan digunakan untuk mengumpulkan argumen-argumen yang diterima oleh fungsi tersebut ke dalam sebuah array. Berikut adalah contoh penggunaan rest parameter pada sebuah fungsi:"
      ],
      "metadata": {
        "id": "VjlAVHj48dyg"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "function jumlahkan(...angka) {\n",
        "  let hasil = 0;\n",
        "  for (let i = 0; i < angka.length; i++) {\n",
        "    hasil += angka[i];\n",
        "  }\n",
        "  return hasil;\n",
        "}\n",
        "\n",
        "console.log(jumlahkan(1, 2, 3, 4, 5)); // Output: 15"
      ],
      "metadata": {
        "id": "7E7d96xF8g0w"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Dalam contoh di atas, rest parameter **...angka** digunakan pada definisi fungsi **jumlahkan** untuk mengumpulkan argumen-argumen yang diterima oleh fungsi tersebut ke dalam sebuah array dengan nama **angka**. Kemudian, elemen-elemen pada array **angka** dijumlahkan dan hasilnya dikembalikan dari fungsi tersebut."
      ],
      "metadata": {
        "id": "k3xVShcI8jAm"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Dapat dilihat bahwa perbedaan utama antara spread operator dan rest parameter adalah pada posisi dan cara penggunaannya. Spread operator digunakan untuk menyebar elemen-elemen dari sebuah array atau objek ke tempat lain, sedangkan rest parameter digunakan untuk mengumpulkan argumen-argumen pada definisi sebuah fungsi ke dalam sebuah array."
      ],
      "metadata": {
        "id": "85kjfxCa8oFo"
      }
    }
  ]
}
