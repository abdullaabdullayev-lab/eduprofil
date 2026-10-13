# EduProfil — başlanğıc layihəsi

Bu qovluq EduProfil-in təhlükəsiz sistemə çevrilməsi üçün başlanğıc skeletidir. Bu, hələ tam işlək/istehsala hazır sistem deyil.

## Seçilən xidmətlər
- GitHub Pages: saytın statik hissəsini yayımlamaq üçün.
- Supabase: giriş, verilənlər bazası və giriş icazələri üçün.

## Vacib təhlükəsizlik qaydaları
1. Real tələbə məlumatlarını demo HTML/JavaScript faylında saxlamayın.
2. Supabase `service_role` açarını heç vaxt brauzer koduna yerləşdirməyin.
3. Tələbələr üçün fərdi hesab və parol/PIN yaradın; yalnız qısa şəxsi kodla girişə güvənməyin.
4. Müəllim hesablarını idarəçi tərəfindən yaradın. İstifadəçilər özlərinə müəllim rolu verə bilməməlidir.
5. RLS siyasətləri yoxlanmadan real məlumat yükləməyin.
6. Təhsil müəssisəsinin icazəsi olmadan tələbələrin şəxsi məlumatlarını sistemə daxil etməyin.

## Quraşdırma planı
1. GitHub hesabı yaradın və bu qovluqdakı faylları yeni repozitoriyaya yükləyin.
2. Supabase hesabında yeni layihə yaradın.
3. Supabase SQL Editor-da `supabase/schema.sql` faylını nəzərdən keçirib icra edin.
4. Supabase layihə URL-i və `anon`/publishable key-i `config.js` faylına yazın. Bu açar ictimai ola bilər; təhlükəsizliyi RLS təmin etməlidir.
5. GitHub Pages-i repozitoriyanın Settings → Pages hissəsindən aktivləşdirin.
6. Yayımlanan URL-ni yoxlayın; QR kodu yalnız bu URL üçün bundan sonra yaradın.

## Hazırda nə var?
- Mobil uyğun başlanğıc giriş səhifəsi.
- Supabase parametrləri üçün boş konfiqurasiya faylı.
- RLS ilə qorunan cədvəllər üçün SQL nümunəsi.

## Nə yoxdur?
- Hazır qeydiyyat/şifrə sıfırlama axını.
- Müəllim hesablarının idarəetmə paneli.
- Real e-arayışın hüquqi təsdiqi/imza mexanizmi.
- Tam yoxlanmış istehsal səviyyəli audit və rate-limit sistemi.

İlk sınağı yalnız saxta məlumatlarla edin.
