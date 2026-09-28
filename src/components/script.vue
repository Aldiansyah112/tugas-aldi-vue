<script>
defineProps(['Nama', 'Harga', 'gambar'])

function tambahKeKeranjang(nama) {
    const suara = new Audio('/audio/notofokasi.mp3')
    suara.play()
    alert(`${nama} ditambahkan ke keranjang!`)
}
</script>

<template>
    <button @click="tambahKeKeranjang(nama)">
        Tambah ke keranjang 
    </button>
</template>