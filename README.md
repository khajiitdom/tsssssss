# hdtSMP64 = Settle (FSMP 4.1.1 + world-collision) + GTSoftBody contact bridge, AVX2 + PDB

Base   : https://github.com/Flob26/Settle-hdtSMP64 @ ab97519 (= upstream v4.1.1 + 2 commits Settle)
Patch  : patch/FSMP_v4.1.1_contact_bridge.patch (GTSoftBody bridge; terbukti apply bersih di atas Settle)

Cara pakai:
1. Upload isi folder ini ke repo GitHub baru (termasuk .github).
2. Actions -> "Build hdtSMP64 = Settle + GTSoftBody..." -> Run workflow.
3. Unduh artifact `hdtSMP64-Settle-GTBridge-avx2-with-pdb`.
4. Taruh hdtSMP64.dll DAN hdtSMP64.pdb bersama di satu folder mod
   (mis. mods\SOFTBODY - Boing Natural\SKSE\Plugins\), dan pastikan mod itu
   menang atas Settle dan Faster HDT-SMP untuk hdtSMP64.dll.
5. Plugin Settle (Settle.dll dkk) tetap dipakai apa adanya dari mod Settle.

Jangan pakai DLL dari build lain bersama PDB ini. DLL dan PDB harus pasangan.
