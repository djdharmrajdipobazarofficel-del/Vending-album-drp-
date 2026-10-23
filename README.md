<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DJ Dharmraj Official - Wedding Album & PSD Store</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body class="bg-slate-950 text-slate-100 font-sans antialiased">

    <!-- Header / Navbar -->
    <header class="sticky top-0 z-50 bg-slate-900/90 backdrop-blur border-b border-slate-800">
        <div class="max-w-7xl mx-auto px-4 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-3">
                <div class="bg-gradient-to-r from-amber-500 to-rose-500 p-2.5 rounded-xl text-white font-bold text-xl shadow-lg">
                    <i class="fa-solid fa-compact-disc fa-spin"></i>
                </div>
                <div>
                    <h1 class="text-xl font-extrabold tracking-wide text-transparent bg-clip-text bg-gradient-to-r from-amber-400 to-rose-400">DJ Dharmraj Official</h1>
                    <p class="text-xs text-slate-400">Wedding PSD & Auto Album Studio</p>
                </div>
            </div>
            <nav class="hidden md:flex space-x-8 font-medium">
                <a href="#store" class="hover:text-amber-400 transition">PSD Store</a>
                <a href="#generator" class="hover:text-amber-400 transition">Auto Album Generator</a>
                <a href="#pricing" class="hover:text-amber-400 transition">Pricing</a>
            </nav>
            <a href="#generator" class="bg-gradient-to-r from-amber-500 to-rose-600 px-5 py-2.5 rounded-xl font-bold shadow-md hover:opacity-90 transition">
                Create Poster
            </a>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="relative py-20 px-4 text-center bg-[radial-gradient(ellipse_at_top,_var(--tw-gradient-stops))] from-slate-900 via-slate-950 to-black border-b border-slate-800">
        <div class="max-w-4xl mx-auto">
            <span class="bg-amber-500/10 text-amber-400 border border-amber-500/20 text-xs px-3 py-1.5 rounded-full font-semibold uppercase tracking-wider">
                🔥 Special Offer: 10 PSDs Absolutely Free!
            </span>
            <h2 class="text-4xl md:text-6xl font-black mt-6 mb-6 leading-tight">
                18,000+ Wedding Album PSD & <span class="text-transparent bg-clip-text bg-gradient-to-r from-amber-400 to-rose-500">Auto Poster Generator</span>
            </h2>
            <p class="text-slate-400 text-lg mb-8 max-w-2xl mx-auto">
                Download high-quality 12x36 wedding album templates or use our automatic poster generator tool to instantly create designs with your own photos!
            </p>
            <div class="flex flex-wrap justify-center gap-4">
                <a href="#store" class="bg-amber-500 hover:bg-amber-600 text-slate-950 px-8 py-3.5 rounded-xl font-bold text-lg shadow-lg transition">
                    Explore Free PSDs
                </a>
                <a href="#generator" class="bg-slate-800 hover:bg-slate-700 text-white border border-slate-700 px-8 py-3.5 rounded-xl font-bold text-lg transition">
                    Try Auto Generator
                </a>
            </div>
        </div>
    </section>

    <!-- PSD Store Section (Free 10 & Paid ₹50) -->
    <section id="store" class="py-16 px-4 max-w-7xl mx-auto">
        <div class="flex justify-between items-end mb-10">
            <div>
                <h3 class="text-3xl font-bold">Wedding Album PSD Templates</h3>
                <p class="text-slate-400 text-sm mt-1">First 10 Templates are 100% Free. Premium templates available at just ₹50[span_3](start_span)[span_3](end_span).</p>
            </div>
            <div class="text-sm bg-slate-900 px-4 py-2 rounded-lg border border-slate-800">
                Total Collection: <span class="text-amber-400 font-bold">18,000+ PSDs</span>
            </div>
        </div>

        <!-- Grid of Templates -->
        <div id="psd-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-5 gap-6">
            <!-- JavaScript will load items here -->
        </div>
    </section>

    <!-- Auto Album & Poster Generator Tool -->
    <section id="generator" class="py-16 px-4 bg-slate-900/50 border-y border-slate-800">
        <div class="max-w-5xl mx-auto">
            <div class="text-center mb-12">
                <h3 class="text-3xl font-bold">Automatic Photo Album & Poster Generator</h3>
                <p class="text-slate-400 mt-2">Upload your photos and instantly generate custom wedding album poster layouts with professional frames.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 bg-slate-900 p-6 md:p-8 rounded-2xl border border-slate-800 shadow-xl">
                <!-- Controls -->
                <div class="space-y-6">
                    <div>
                        <label class="block text-sm font-semibold mb-2">1. Select Template Layout</label>
                        <select id="layout-select" class="w-full bg-slate-950 border border-slate-700 rounded-xl p-3 text-sm focus:outline-none focus:border-amber-500">
                            <option value="layout-1">Royal Red Wedding Spread (12x36)</option>
                            <option value="layout-2">Golden Elegance Border</option>
                            <option value="layout-3">Modern Floral Fusion</option>
                        </select>
                    </div>

                    <div>
                        <label class="block text-sm font-semibold mb-2">2. Upload Your Photos</label>
                        <input type="file" id="image-upload" multiple accept="image/*" class="w-full text-sm text-slate-400 file:mr-4 file:py-2 file:px-4 file:rounded-xl file:border-0 file:text-sm file:font-semibold file:bg-amber-500 file:text-slate-955 hover:file:bg-amber-600 cursor-pointer">
                    </div>

                    <div>
                        <label class="block text-sm font-semibold mb-2">3. Couple / Album Title</label>
                        <input type="text" id="album-title" value="Rahul & Priya Wedding" class="w-full bg-slate-950 border border-slate-700 rounded-xl p-3 text-sm focus:outline-none focus:border-amber-500">
                    </div>

                    <button onclick="generatePoster()" class="w-full bg-gradient-to-r from-amber-500 to-rose-600 text-slate-950 font-bold py-3.5 rounded-xl shadow-lg hover:opacity-90 transition">
                        Generate Album Poster
                    </button>
                </div>

                <!-- Preview Box -->
                <div class="md:col-span-2 bg-slate-950 rounded-xl border border-slate-800 p-4 flex flex-col justify-center items-center relative min-h-[350px]">
                    <div id="poster-preview" class="w-full h-full flex flex-col items-center justify-center text-center border-2 border-dashed border-slate-700 rounded-lg p-6">
                        <i class="fa-regular fa-image text-4xl text-slate-600 mb-3"></i>
                        <p class="text-slate-500 text-sm">Upload photos and click 'Generate Album Poster' to see live preview here.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-8 px-4 text-center text-sm text-slate-500 border-t border-slate-800">
        <p>&copy; 2026 DJ Dharmraj Official. All Rights Reserved. Built for Professional Photographers & Designers.</p>
    </footer>

    <!-- JavaScript for Dynamic Store & Generator Logic -->
    <script>
        // Generate 10 Free PSDs and subsequent Paid PSDs (₹50)
        const storeGrid = document.getElementById('psd-grid');
        for (let i = 1; i <= 15; i++) {
            let isFree = i <= 10;
            let cardHTML = `
                <div class="bg-slate-900 rounded-2xl overflow-hidden border border-slate-800 hover:border-amber-500/50 transition flex flex-col justify-between">
                    <div>
                        <div class="h-40 bg-gradient-to-br from-slate-800 to-slate-950 relative flex items-center justify-center">
                            <span class="absolute top-3 left-3 ${isFree ? 'bg-emerald-500/20 text-emerald-400 border-emerald-500/30' : 'bg-amber-500/20 text-amber-400 border-amber-500/30'} border text-xs px-2.5 py-1 rounded-full font-bold">
                                ${isFree ? 'FREE' : '₹50'}
                            </span>
                            <i class="fa-solid fa-photo-film text-3xl text-slate-600"></i>
                        </div>
                        <div class="p-4">
                            <h4 class="font-bold text-sm">Wedding Spread #${i}</h4>
                            <p class="text-xs text-slate-400 mt-1">12x36 PSD • Fully Layered</p>
                        </div>
                    </div>
                    <div class="p-4 pt-0">
                        <button onclick="downloadOrBuy(${i}, ${isFree})" class="w-full py-2.5 rounded-xl font-bold text-xs ${isFree ? 'bg-emerald-600 hover:bg-emerald-500 text-white' : 'bg-amber-500 hover:bg-amber-600 text-slate-950'} transition">
                            ${isFree ? 'Instant Download Free' : 'Buy Now ₹50'}
                        </button>
                    </div>
                </div>
            `;
            storeGrid.innerHTML += cardHTML;
        }

        function downloadOrBuy(id, isFree) {
            if(isFree) {
                alert(`Template #${id} download started successfully! (Free)` );
            } else {
                alert(`Redirecting to secure checkout for Template #${id} at ₹50[span_4](start_span)[span_4](end_span)...`);
            }
        }

        // Poster Generator Script
        function generatePoster() {
            const title = document.getElementById('album-title').value;
            const fileInput = document.getElementById('image-upload');
            const previewBox = document.getElementById('poster-preview');

            if(fileInput.files.length === 0) {
                alert('Please upload at least one photo for the album poster!');
                return;
            }

            let previewHTML = `<div class="w-full text-left"><h4 class="text-amber-400 font-bold mb-3 text-lg">${title}</h4><div class="grid grid-cols-2 sm:grid-cols-3 gap-3">`;
            
            for(let i=0; i < Math.min(fileInput.files.length, 6); i++) {
                let imageUrl = URL.createObjectURL(fileInput.files[i]);
                previewHTML += `<div class="h-28 bg-slate-900 rounded-lg overflow-hidden border border-slate-700"><img src="${imageUrl}" class="w-full h-full object-cover"></div>`;
            }

            previewHTML += `</div><p class="text-xs text-emerald-400 mt-4"><i class="fa-solid fa-circle-check"></i> Poster generated successfully with high quality settings!</p></div>`;
            previewBox.innerHTML = previewHTML;
        }
    </script>
</body>
</html>
