<script>
    let disabled = $state(true);

    let src = "https://scontent.fmnl4-2.fna.fbcdn.net/v/t39.30808-6/654853973_1727167654926513_1416734826057444183_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeGWv2nOimf4ouPh-pd2sjTgxjga6J_xjCXGOBron_GMJUjX1XMGRnHvlOozBCY4JicZo2keax-IbPD0Gm2GrPUt&_nc_ohc=kbchkqu5AmUQ7kNvwEAcbKj&_nc_oc=Adqx22SoY7DLLeDFrE-grGRbkeqgBJDnxAft1dKZp78bNJW8FR9l1pCES_pBq2Wm1du6h8WzAz0DyhPKJqU1iQ5v&_nc_zt=23&_nc_ht=scontent.fmnl4-2.fna&_nc_gid=ATqfkzUZ042ohTkPQpMAOw&_nc_ss=7b2a8&oh=00_Af6QdHHtSK6qWkbhWJ-Cym1nCtInhXW3eisqZ83Bkfufng&oe=6A1A5F47";
</script>

<div class="flex justify-center items-center h-screen">
    <div class="text-center">
        <button 
        {disabled}
        class = "px-4 py-2 bg-blue-500 text-white rounded disabled:bg-gray-400"
        onclick = {()=>{
            console.log("Button Clicked!");
        }}>Click me</button>

        <button 
        class = "px-4 py-2 bg-blue-500 text-white rounded"
        onclick = {()=>{
            disabled = !disabled;
        }}>Toggle</button>

        <img {src} alt="My image" width="200"/>
    </div>
</div>