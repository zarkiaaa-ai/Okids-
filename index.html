import React, { useState, useEffect, useMemo, useCallback } from "react";
import {
  Home, Package, Newspaper, Heart, Menu, X, ArrowLeft, MapPin, Phone, Mail,
  Award, Building2, Users, ChefHat, ShieldCheck, Search, Plus, Pencil, Trash2,
  Lock, ExternalLink, Instagram, Facebook, Youtube, Linkedin, Clock, Scale,
  Info, ChevronLeft, Factory, BookMarked, GitCompareArrows, Sparkles, Check,
  LogOut, Image as ImageIcon
} from "lucide-react";

/* ============================== بيانات حقيقية موثقة (من الموقع الرسمي goumidigroupe.com) ============================== */
const SOURCE_SITE = "https://www.goumidigroupe.com";
const LOGO = "https://www.goumidigroupe.com/images/logo.png";

const DEFAULT_DATA = {
  company: {
    name: "Groupe Industriel GOUMIDI — G.I.G. SPA",
    brand: "OKID'S",
    founded: "28 يوليو 1998",
    founder: "الراحل نور الدين قُوميدي",
    sector: "الصناعات الغذائية — منتجات الألبان ومشتقاتها",
    hq: "البليدة، الجزائر",
    address: "Zone Industrielle, site 02 n°38 - 09015 Ouled Yaich, Blida, Algérie",
    phone: "+213 (0) 25 26 90 77",
    email: "commercial@goumidigroupe.com",
    employeesRange: "201–500 موظف تقريبًا",
    iso: "ISO 9001 V2008 — مارس 2009",
    about:
      "Groupe Industriel GOUMIDI-G.I.G. SPA شركة جزائرية متخصصة في تصنيع وتسويق منتجات الألبان ومشتقاتها. تأسست في 28 يوليو 1998 على يد الراحل نور الدين قُوميدي. ابتداءً من سنة 2000 اتجهت الشركة نحو إنتاج الجبن المطبوخ بتشكيلة متنوعة (حصص، أصابع...) تحت علامة OKID'S، بفضل تقنيات حديثة وخبرة متراكمة. كما تخصصت الشركة في تعبئة حليب البودرة، وبودرة الشوكولاتة، ورقائق البطاطا. وحصلت على شهادة ISO 9001 V2008 في مارس 2009. اليوم تحتل الشركة مكانة على المستويين الوطني والدولي، ولديها ثلاث شركات فرعية أخرى تعمل في قطاع الصناعات الغذائية.",
    socials: {
      instagram: "https://www.instagram.com/okidsfromage",
      facebook: "https://www.facebook.com/okidsalgerie",
      linkedin: "https://dz.linkedin.com/company/o-kids",
      youtube: "https://www.youtube.com/@OkidsFromage-b4m",
      tiktok: "https://www.tiktok.com/@okids.fromage",
    },
  },
  timeline: [
    { year: "1998", title: "التأسيس", text: "تأسيس Groupe Industriel GOUMIDI (G.I.G. SPA) في 28 يوليو 1998 على يد الراحل نور الدين قُوميدي." },
    { year: "2000", title: "ميلاد علامة OKID'S", text: "توجّه الشركة نحو إنتاج الجبن المطبوخ بتشكيلة متنوعة (حصص، أصابع) تحت علامة OKID'S." },
    { year: "2009", title: "شهادة الجودة", text: "الحصول على شهادة ISO 9001 V2008 في مارس 2009." },
    { year: "اليوم", title: "حضور وطني ودولي", text: "تحتل الشركة مكانة على المستويين الوطني والدولي، ولديها 3 شركات فرعية أخرى في قطاع الصناعات الغذائية." },
  ],
  products: [
    { id: "okids-portion", brand: "OKID'S", type: "جبن مطبوخ — حصص", name: "OKID'S Portion", desc: "جبن مطبوخ على شكل حصص فردية بعلامة OKID'S.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K42E1Q93DQAM9WR39VAJM7D5.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "يُحفظ في الثلاجة", expiry: "موضّح على العبوة" },
    { id: "okids-barre", brand: "OKID'S", type: "جبن مطبوخ — أصابع/قضبان", name: "OKID'S Barre de Fromage", desc: "جبن مطبوخ على شكل أصابع (بار) بعلامة OKID'S.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K42EJHJ0SDPX0QNEHM15457H.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "يُحفظ في الثلاجة", expiry: "موضّح على العبوة" },
    { id: "okids-poudre", brand: "OKID'S", type: "حليب بودرة", name: "OKID'S Poudre de Lait", desc: "منتج حليب مجفف (بودرة) بعلامة OKID'S.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K4GV025FC17DXM14M1RGZMEJ.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "مكان جاف وبارد", expiry: "موضّح على العبوة" },
    { id: "pot-okids", brand: "OKID'S", type: "جبن — وعاء (Pot)", name: "Pot OKID'S", desc: "جبن OKID'S معبأ في وعاء (Pot).", img: "https://www.goumidigroupe.com/storage/products/gallery/01K4GV86R2X56K85XGJWAYRNED.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "يُحفظ في الثلاجة", expiry: "موضّح على العبوة" },
    { id: "bravo-portion", brand: "BRAVO", type: "جبن مطبوخ — حصص", name: "Bravo Portion", desc: "جبن مطبوخ على شكل حصص فردية بعلامة Bravo.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K5TWK64R0YHGPYQT5W0E9AEG.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "يُحفظ في الثلاجة", expiry: "موضّح على العبوة" },
    { id: "bravo-barre", brand: "BRAVO", type: "جبن مطبوخ — أصابع/قضبان", name: "Bravo Barre", desc: "جبن مطبوخ على شكل أصابع بعلامة Bravo.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K5S67XE5MVNGCHV3MXBC4XQ0.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "يُحفظ في الثلاجة", expiry: "موضّح على العبوة" },
    { id: "bravo-seau", brand: "BRAVO", type: "جبن مطبوخ — سطل (Seau)", name: "Bravo Seau", desc: "جبن مطبوخ معبأ في سطل بعلامة Bravo.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K5TWE241FYSD0WK6XCVQX801.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "يُحفظ في الثلاجة", expiry: "موضّح على العبوة" },
    { id: "bravo-poudre", brand: "BRAVO", type: "حليب بودرة", name: "Bravo Poudre de Lait", desc: "منتج حليب مجفف (بودرة) بعلامة Bravo.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K5TWHBHR5W68XHJ2YRJ78XRW.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "مكان جاف وبارد", expiry: "موضّح على العبوة" },
    { id: "pot-fromages", brand: "BRAVO", type: "جبن — وعاء (Pot)", name: "Pot Fromages", desc: "جبن معبأ في وعاء (Pot) بعلامة Bravo.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K5TW10S7EY1YTFQE7F7VJCS8.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "يُحفظ في الثلاجة", expiry: "موضّح على العبوة" },
    { id: "tasty-portions", brand: "TASTY", type: "جبن مطبوخ — حصص", name: "Tasty Portions", desc: "جبن مطبوخ على شكل حصص فردية بعلامة Tasty.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K5TWQTM20JAKNKRQMPF6X3GG.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "يُحفظ في الثلاجة", expiry: "موضّح على العبوة" },
    { id: "tasty-seau", brand: "TASTY", type: "جبن مطبوخ — سطل (Seau)", name: "Tasty Seau", desc: "جبن مطبوخ معبأ في سطل بعلامة Tasty.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K5TWRVKN9V6E64W0CEXX7C0H.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "يُحفظ في الثلاجة", expiry: "موضّح على العبوة" },
    { id: "tasty-barre", brand: "TASTY", type: "جبن مطبوخ — أصابع/قضبان", name: "Tasty Barre", desc: "جبن مطبوخ على شكل أصابع بعلامة Tasty.", img: "https://www.goumidigroupe.com/storage/products/gallery/01K5S4F2S47AAH2K8GHEVMP5HH.png", ingredients: "ماء معالَج، بودرة حليب شيدر، ملح طعام.", sizes: "غير موثّقة رسميًا بعد", storage: "يُحفظ في الثلاجة", expiry: "موضّح على العبوة" },
  ],
  news: [
    { id: "fia-2026", title: "FIA 2026", date: "2026-06-22", place: "قصر المعارض – الصنوبر البحري", desc: "ندعوكم لزيارة جناحنا واكتشاف عالم أوكدس المليء بالنكهات والأنشطة والمفاجآت لكل أفراد العائلة.", img: LOGO, link: "https://www.goumidigroupe.com/blogpost/fia-2026" },
    { id: "street-food", title: "Street Food Algiers Festival", date: "2026-06-11", place: "الجزائر العاصمة", desc: "مشاركة أوكدس في Algiers Street Food Festival.", img: LOGO, link: "https://www.goumidigroupe.com/blogpost/street-food-algiers-festival" },
    { id: "ifsa", title: "IFSA — المعرض الدولي للصناعات الغذائية بتونس", date: "2026-06-09", place: "تونس", desc: "مشاركة أوكدس في المعرض الدولي للصناعات الغذائية بتونس.", img: LOGO, link: "https://www.goumidigroupe.com" },
  ],
  recipes: [
    { id: "cake-fromage", title: "Cake au fromage", time: "00:19:00", product: "منتجات جبن OKID'S", img: "https://www.goumidigroupe.com/storage/recipes/01K1B23NZT1J0ZM1Q3YWX9VWCQ.png", ingredients: "التفاصيل الكاملة على الموقع الرسمي.", steps: "التفاصيل الكاملة على الموقع الرسمي." },
    { id: "pdt-farcie", title: "Pomme de terre farcie", time: "00:20:00", product: "منتجات جبن OKID'S", img: "https://www.goumidigroupe.com/storage/recipes/01K1B28NHW52BPJ6QB4HH6FTCZ.png", ingredients: "التفاصيل الكاملة على الموقع الرسمي.", steps: "التفاصيل الكاملة على الموقع الرسمي." },
    { id: "croquettes", title: "Croquettes de fromage", time: "00:22:22", product: "منتجات جبن OKID'S", img: "https://www.goumidigroupe.com/storage/recipes/01K1B29RZVZBSXATFQ6GQKBS4B.png", ingredients: "التفاصيل الكاملة على الموقع الرسمي.", steps: "التفاصيل الكاملة على الموقع الرسمي." },
  ],
  branches: {
    note: "تملك المجموعة 3 شركات فرعية أخرى في قطاع الصناعات الغذائية حسب الموقع الرسمي، إلا أن أسماءها وأنشطتها التفصيلية غير منشورة رسميًا بعد.",
  },
  sources: [
    { label: "الموقع الرسمي — الرئيسية", url: "https://www.goumidigroupe.com" },
    { label: "الموقع الرسمي — من نحن", url: "https://www.goumidigroupe.com/about" },
    { label: "الموقع الرسمي — المنتجات", url: "https://www.goumidigroupe.com/produits" },
    { label: "الموقع الرسمي — الوصفات", url: "https://www.goumidigroupe.com/recipes" },
    { label: "الموقع الرسمي — الأخبار", url: "https://www.goumidigroupe.com/blogpost" },
    { label: "الموقع الرسمي — التواصل", url: "https://www.goumidigroupe.com/contact" },
    { label: "LinkedIn — O'KIDS", url: "https://dz.linkedin.com/company/o-kids" },
  ],
};

/* ==============================
   نظام الصور: يحاول أولًا الصورة المحلية من مجلد assets (إن وُجدت)،
   ثم يحاول رابط الموقع الرسمي، وإن فشل الاثنان يعرض بطاقة أنيقة
   بدل أيقونة الصورة المكسورة — لا يوجد src فارغ أبدًا.
   ملاحظة: لتفعيل الصور المحلية ضع الملفات في:
   src/assets/products/<id>.png  (نفس الـ id الموجود في بيانات المنتج)
   src/assets/news/<id>.png · src/assets/recipes/<id>.png
   ============================== */
function useImageSource(id, folder, remoteSrc) {
  const [tier, setTier] = useState(0);
  const sources = useMemo(
    () => [`./assets/${folder}/${id}.png`, remoteSrc].filter(Boolean),
    [id, folder, remoteSrc]
  );
  const failed = tier >= sources.length;
  return { src: failed ? null : sources[tier], failed, onError: () => setTier((t) => t + 1) };
}

function SmartImage({ id, folder = "products", remoteSrc, alt, className, boxClassName, onClick, iconSize = 24 }) {
  const { src, failed, onError } = useImageSource(id, folder, remoteSrc);
  if (failed) {
    return (
      <div className={"img-fallback " + (boxClassName || "")} onClick={onClick} role={onClick ? "button" : undefined}>
        <ImageIcon size={iconSize} />
        <span>صورة المنتج غير متوفرة حاليًا</span>
      </div>
    );
  }
  return (
    <img
      src={src}
      alt={alt}
      className={className}
      loading="lazy"
      referrerPolicy="no-referrer"
      onClick={onClick}
      onError={onError}
    />
  );
}

const BRAND_COLOR = { "OKID'S": "#B5222E", "BRAVO": "#1D4E89", "TASTY": "#D69A22" };
const BRAND_TINT = { "OKID'S": "#FBEAEA", "BRAVO": "#E9F0F8", "TASTY": "#FBF1E1" };

const NAV_MAIN = [
  { id: "home", label: "الرئيسية", icon: Home },
  { id: "products", label: "المنتجات", icon: Package },
  { id: "news", label: "الأخبار", icon: Newspaper },
  { id: "favorites", label: "المفضلة", icon: Heart },
  { id: "more", label: "المزيد", icon: Menu },
];

const MORE_LINKS = [
  { id: "about", label: "عن الشركة", icon: Building2 },
  { id: "history", label: "تاريخ الشركة", icon: Clock },
  { id: "awards", label: "الجوائز والإنجازات", icon: Award },
  { id: "compare", label: "مقارنة المنتجات", icon: GitCompareArrows },
  { id: "recipes", label: "الوصفات", icon: ChefHat },
  { id: "quality", label: "عن الجودة", icon: ShieldCheck },
  { id: "branches", label: "الشركات والفروع", icon: Factory },
  { id: "employees", label: "الموظفون", icon: Users },
  { id: "location", label: "موقع الشركة", icon: MapPin },
  { id: "contact", label: "تواصل معنا", icon: Phone },
  { id: "sources", label: "المصادر والمراجع", icon: BookMarked },
  { id: "admin", label: "لوحة التحكم (Admin)", icon: Lock },
];

/* ============================== Storage helpers ============================== */
async function loadData() {
  try {
    const res = await window.storage.get("okids:data", false);
    if (res && res.value) return JSON.parse(res.value);
  } catch (e) { /* not found yet */ }
  return null;
}
async function saveData(data) {
  try { await window.storage.set("okids:data", JSON.stringify(data), false); } catch (e) { /* ignore */ }
}
async function loadFavs() {
  try {
    const res = await window.storage.get("okids:favs", false);
    if (res && res.value) return JSON.parse(res.value);
  } catch (e) {}
  return [];
}
async function saveFavs(favs) {
  try { await window.storage.set("okids:favs", JSON.stringify(favs), false); } catch (e) {}
}

/* ============================== UI Bits ============================== */
function Pill({ children, color }) {
  return (
    <span className="pill" style={{ background: color, color: "#fff" }}>{children}</span>
  );
}

function SectionTitle({ eyebrow, title, sub }) {
  return (
    <div className="section-title">
      {eyebrow && <div className="eyebrow"><span className="dot" />{eyebrow}</div>}
      <h2>{title}</h2>
      {sub && <p className="sub">{sub}</p>}
    </div>
  );
}

function TopBar({ title, onBack, right }) {
  return (
    <header className="topbar">
      {onBack ? (
        <button className="icon-btn" onClick={onBack} aria-label="رجوع"><ArrowLeft size={20} /></button>
      ) : (
        <img src={LOGO} alt="OKID'S" className="topbar-logo" referrerPolicy="no-referrer" onError={(e)=>{e.currentTarget.style.display='none';}} />
      )}
      <h1>{title}</h1>
      <div className="topbar-right">{right}</div>
    </header>
  );
}

function ProductCard({ p, onOpen, fav, onToggleFav, compareMode, selected, onSelect }) {
  const color = BRAND_COLOR[p.brand] || "#8C1D2B";
  return (
    <div className="product-card" style={{ borderColor: selected ? color : "transparent" }}>
      <div className="product-band" style={{ background: color }}>{p.brand}</div>
      <button className="fav-btn" onClick={() => onToggleFav(p.id)} aria-label="مفضلة">
        <Heart size={18} fill={fav ? "#E0455A" : "none"} color={fav ? "#E0455A" : "#8a8478"} />
      </button>
      <div className="product-img-wrap" onClick={() => (compareMode ? onSelect(p.id) : onOpen(p.id))}>
        <SmartImage id={p.id} remoteSrc={p.img} alt={p.name} className="prod-img" boxClassName="prod-img-box" iconSize={22} />
      </div>
      <div className="product-body" onClick={() => (compareMode ? onSelect(p.id) : onOpen(p.id))}>
        <div className="product-type">{p.type}</div>
        <div className="product-name">{p.name}</div>
        <div className="product-desc">{p.desc}</div>
      </div>
      {compareMode ? (
        <button className={"btn-outline small" + (selected ? " active" : "")} onClick={() => onSelect(p.id)} style={{ borderColor: color, color: selected ? "#fff" : color, background: selected ? color : "transparent" }}>
          {selected ? <><Check size={14}/> محدد</> : "اختيار للمقارنة"}
        </button>
      ) : (
        <button className="btn-outline small" style={{ borderColor: color, color }} onClick={() => onOpen(p.id)}>التفاصيل</button>
      )}
    </div>
  );
}

/* ============================== App ============================== */
export default function App() {
  const [data, setData] = useState(DEFAULT_DATA);
  const [ready, setReady] = useState(false);
  const [screen, setScreen] = useState("home");
  const [prevScreen, setPrevScreen] = useState("home");
  const [moreSheet, setMoreSheet] = useState(false);
  const [activeProduct, setActiveProduct] = useState(null);
  const [activeBrandFilter, setActiveBrandFilter] = useState("الكل");
  const [query, setQuery] = useState("");
  const [favs, setFavs] = useState([]);
  const [compareIds, setCompareIds] = useState([]);
  const [adminAuthed, setAdminAuthed] = useState(false);
  const [adminPass, setAdminPass] = useState("");
  const [adminError, setAdminError] = useState("");
  const [toast, setToast] = useState("");

  useEffect(() => {
    (async () => {
      const d = await loadData();
      const f = await loadFavs();
      if (d) setData(d); else await saveData(DEFAULT_DATA);
      if (f) setFavs(f);
      setReady(true);
    })();
  }, []);

  const showToast = useCallback((msg) => {
    setToast(msg);
    setTimeout(() => setToast(""), 2200);
  }, []);

  const go = (s) => { setPrevScreen(screen); setScreen(s); setMoreSheet(false); window.scrollTo(0,0); };
  const openProduct = (id) => { setActiveProduct(id); go("productDetail"); };

  const toggleFav = async (id) => {
    const next = favs.includes(id) ? favs.filter(x => x !== id) : [...favs, id];
    setFavs(next);
    await saveFavs(next);
  };

  const updateData = async (mutator) => {
    setData(prev => {
      const next = mutator(structuredClone(prev));
      saveData(next);
      return next;
    });
  };

  const filteredProducts = useMemo(() => {
    let list = data.products;
    if (activeBrandFilter !== "الكل") list = list.filter(p => p.brand === activeBrandFilter);
    if (query.trim()) {
      const q = query.trim().toLowerCase();
      list = list.filter(p =>
        p.name.toLowerCase().includes(q) || p.type.includes(q) || p.brand.toLowerCase().includes(q) ||
        p.desc.includes(q) || (q.includes("جبن") && true === true && (p.type.includes("جبن"))) ||
        (q.includes("حليب") && p.type.includes("حليب"))
      );
    }
    return list;
  }, [data.products, activeBrandFilter, query]);

  const product = useMemo(() => data.products.find(p => p.id === activeProduct), [data.products, activeProduct]);
  const compareProducts = compareIds.map(id => data.products.find(p => p.id === id)).filter(Boolean);

  const toggleCompareSelect = (id) => {
    setCompareIds(prev => {
      if (prev.includes(id)) return prev.filter(x => x !== id);
      if (prev.length >= 2) return [prev[1], id];
      return [...prev, id];
    });
  };

  if (!ready) {
    return (
      <div className="app-shell" dir="rtl"><Style />
        <div className="loading-screen">
          <img src={LOGO} alt="OKID'S" referrerPolicy="no-referrer" style={{ width: 96, opacity: 0.9 }} />
          <div className="spinner" />
        </div>
      </div>
    );
  }

  return (
    <div className="app-shell" dir="rtl">
      <Style />
      <div className="app-frame">
        {screen === "home" && <HomeScreen data={data} go={go} openProduct={openProduct} />}
        {screen === "about" && <AboutScreen data={data} go={go} />}
        {screen === "history" && <HistoryScreen data={data} go={go} />}
        {screen === "products" && (
          <ProductsScreen
            products={filteredProducts} allProducts={data.products} go={go} openProduct={openProduct}
            brandFilter={activeBrandFilter} setBrandFilter={setActiveBrandFilter}
            query={query} setQuery={setQuery} favs={favs} toggleFav={toggleFav}
          />
        )}
        {screen === "productDetail" && product && (
          <ProductDetailScreen product={product} go={go} favs={favs} toggleFav={toggleFav} />
        )}
        {screen === "awards" && <AwardsScreen go={go} data={data} />}
        {screen === "news" && <NewsScreen data={data} go={go} />}
        {screen === "location" && <LocationScreen data={data} go={go} />}
        {screen === "employees" && <EmployeesScreen data={data} go={go} />}
        {screen === "branches" && <BranchesScreen data={data} go={go} />}
        {screen === "recipes" && <RecipesScreen data={data} go={go} />}
        {screen === "quality" && <QualityScreen data={data} go={go} />}
        {screen === "contact" && <ContactScreen data={data} go={go} />}
        {screen === "favorites" && (
          <FavoritesScreen products={data.products} favs={favs} go={go} openProduct={openProduct} toggleFav={toggleFav} />
        )}
        {screen === "compare" && (
          <CompareScreen products={data.products} compareIds={compareIds} toggleCompareSelect={toggleCompareSelect} compareProducts={compareProducts} go={go} />
        )}
        {screen === "sources" && <SourcesScreen data={data} go={go} />}
        {screen === "admin" && (
          <AdminScreen
            go={go} data={data} updateData={updateData}
            authed={adminAuthed} setAuthed={setAdminAuthed}
            pass={adminPass} setPass={setAdminPass} error={adminError} setError={setAdminError}
            showToast={showToast}
          />
        )}
      </div>

      {toast && <div className="toast">{toast}</div>}

      {moreSheet && (
        <div className="sheet-backdrop" onClick={() => setMoreSheet(false)}>
          <div className="sheet" onClick={(e) => e.stopPropagation()}>
            <div className="sheet-handle" />
            <div className="sheet-title">المزيد من موسوعة OKID'S</div>
            <div className="sheet-grid">
              {MORE_LINKS.map(l => (
                <button key={l.id} className="sheet-item" onClick={() => go(l.id)}>
                  <l.icon size={20} />
                  <span>{l.label}</span>
                </button>
              ))}
            </div>
          </div>
        </div>
      )}

      <nav className="bottom-nav">
        {NAV_MAIN.map(item => {
          const isActive = item.id === "more" ? moreSheet : screen === item.id;
          return (
            <button
              key={item.id}
              className={"nav-btn" + (isActive ? " active" : "")}
              onClick={() => (item.id === "more" ? setMoreSheet(true) : go(item.id))}
            >
              <item.icon size={20} />
              <span>{item.label}</span>
            </button>
          );
        })}
      </nav>
    </div>
  );
}

/* ============================== Screens ============================== */
function HomeScreen({ data, go, openProduct }) {
  const c = data.company;
  return (
    <div className="screen home-screen">
      <div className="hero">
        <img src={LOGO} alt="OKID'S" className="hero-logo" referrerPolicy="no-referrer" onError={(e)=>{e.currentTarget.style.display='none';}} />
        <div className="hero-badge"><Sparkles size={13}/> موسوعة الشركة ومنتجاتها</div>
        <h1>عالم <span>OKID'S</span> للجبن والألبان</h1>
        <p>منصة تعريفية رسمية بمجموعة Groupe Industriel GOUMIDI وعلاماتها OKID'S · BRAVO · TASTY — كل المعلومات من مصادر موثقة.</p>
        <div className="hero-actions">
          <button className="btn-primary" onClick={() => go("products")}>اكتشف منتجاتنا</button>
          <button className="btn-ghost" onClick={() => go("history")}>تاريخ الشركة</button>
        </div>
        <div className="hero-links">
          <button onClick={() => go("about")}>عن الشركة</button>
          <button onClick={() => go("location")}>مواقعنا</button>
          <button onClick={() => go("news")}>الأخبار</button>
        </div>
      </div>

      <div className="stats-strip">
        <div className="stat"><span className="stat-num">1998</span><span className="stat-label">سنة التأسيس</span></div>
        <div className="stat"><span className="stat-num">201–500</span><span className="stat-label">عدد الموظفين تقريبًا</span></div>
        <div className="stat"><span className="stat-num">3</span><span className="stat-label">علامات تجارية</span></div>
        <div className="stat"><span className="stat-num">{c.hq}</span><span className="stat-label">المقر</span></div>
      </div>

      <SectionTitle eyebrow="Nos Gammes" title="أحدث المنتجات" />
      <div className="h-scroll">
        {data.products.slice(0, 6).map(p => (
          <div key={p.id} className="mini-card" onClick={() => openProduct(p.id)}>
            <div className="mini-band" style={{ background: BRAND_COLOR[p.brand] }}>{p.brand}</div>
            <SmartImage id={p.id} remoteSrc={p.img} alt={p.name} className="mini-img" boxClassName="mini-img-box" iconSize={18} />
            <div className="mini-name">{p.name}</div>
          </div>
        ))}
      </div>
      <button className="link-more" onClick={() => go("products")}>عرض كل المنتجات <ChevronLeft size={16}/></button>

      <SectionTitle eyebrow="Actualités" title="آخر الأخبار والمعارض" />
      <div className="news-list">
        {data.news.slice(0, 2).map(n => (
          <div key={n.id} className="news-row" onClick={() => go("news")}>
            <div className="news-row-date">{n.date}</div>
            <div>
              <div className="news-row-title">{n.title}</div>
              <div className="news-row-place"><MapPin size={12}/> {n.place}</div>
            </div>
          </div>
        ))}
      </div>
      <button className="link-more" onClick={() => go("news")}>كل الأخبار <ChevronLeft size={16}/></button>

      <div className="bottom-spacer" />
    </div>
  );
}

function AboutScreen({ data, go }) {
  const c = data.company;
  return (
    <div className="screen">
      <TopBar title="عن الشركة" onBack={() => go("home")} />
      <div className="content-pad">
        <div className="card soft">
          <p className="lead">{c.about}</p>
        </div>
        <div className="info-grid">
          <InfoRow icon={Building2} label="الاسم الكامل" value={c.name} />
          <InfoRow icon={Clock} label="تاريخ التأسيس" value={c.founded} />
          <InfoRow icon={Users} label="المؤسس" value={c.founder} />
          <InfoRow icon={Package} label="القطاع" value={c.sector} />
          <InfoRow icon={MapPin} label="المقر" value={c.hq} />
          <InfoRow icon={ShieldCheck} label="شهادة الجودة" value={c.iso} />
        </div>
        <SourceNote text="المصدر: الموقع الرسمي لمجموعة GOUMIDI — صفحة «Présentation»." />
      </div>
    </div>
  );
}

function HistoryScreen({ data, go }) {
  return (
    <div className="screen">
      <TopBar title="تاريخ الشركة" onBack={() => go("home")} />
      <div className="content-pad">
        <div className="timeline">
          {data.timeline.map((t, i) => (
            <div className="tl-item" key={i}>
              <div className="tl-dot" />
              <div className="tl-year">{t.year}</div>
              <div className="tl-card">
                <div className="tl-title">{t.title}</div>
                <p>{t.text}</p>
              </div>
            </div>
          ))}
        </div>
        <p className="hint">سيتم إضافة سنوات وأحداث جديدة فور توفر مصدر رسمي موثّق لها.</p>
      </div>
    </div>
  );
}

function ProductsScreen({ products, allProducts, go, openProduct, brandFilter, setBrandFilter, query, setQuery, favs, toggleFav }) {
  const brands = ["الكل", "OKID'S", "BRAVO", "TASTY"];
  return (
    <div className="screen">
      <TopBar title="منتجات OKID'S" onBack={() => go("home")} />
      <div className="content-pad">
        <div className="search-box">
          <Search size={16} />
          <input placeholder="ابحث: جبن، OKID'S، Bravo، حليب…" value={query} onChange={(e) => setQuery(e.target.value)} />
        </div>
        <div className="chip-row">
          {brands.map(b => (
            <button key={b} className={"chip" + (brandFilter === b ? " active" : "")} style={brandFilter === b && b !== "الكل" ? { background: BRAND_COLOR[b], borderColor: BRAND_COLOR[b] } : {}} onClick={() => setBrandFilter(b)}>{b}</button>
          ))}
        </div>
        <div className="product-grid">
          {products.map(p => (
            <ProductCard key={p.id} p={p} onOpen={openProduct} fav={favs.includes(p.id)} onToggleFav={toggleFav} />
          ))}
        </div>
        {products.length === 0 && <EmptyState text="لا توجد منتجات مطابقة للبحث." />}
      </div>
    </div>
  );
}

function ProductDetailScreen({ product: p, go, favs, toggleFav }) {
  const color = BRAND_COLOR[p.brand];
  const [lightbox, setLightbox] = useState(false);
  return (
    <div className="screen">
      <TopBar title={p.name} onBack={() => go("products")} />
      <div className="pd-hero" style={{ background: BRAND_TINT[p.brand] }}>
        <SmartImage id={p.id} remoteSrc={p.img} alt={p.name} className="pd-hero-img" boxClassName="pd-hero-fallback" iconSize={30} onClick={() => setLightbox(true)} />
        <div className="pd-hero-hint"><Search size={12}/> اضغط للتكبير</div>
      </div>
      {lightbox && (
        <div className="lightbox-backdrop" onClick={() => setLightbox(false)}>
          <button className="lightbox-close" onClick={() => setLightbox(false)} aria-label="إغلاق"><X size={20}/></button>
          <SmartImage id={p.id} remoteSrc={p.img} alt={p.name} className="lightbox-img" boxClassName="lightbox-fallback" iconSize={36} />
        </div>
      )}
      <div className="content-pad">
        <div className="pd-head">
          <Pill color={color}>{p.brand}</Pill>
          <button className="icon-btn" onClick={() => toggleFav(p.id)}>
            <Heart size={20} fill={favs.includes(p.id) ? "#E0455A" : "none"} color={favs.includes(p.id) ? "#E0455A" : "#8a8478"} />
          </button>
        </div>
        <h2 className="pd-title">{p.name}</h2>
        <div className="pd-type">{p.type}</div>
        <p className="pd-desc">{p.desc}</p>
        <div className="pd-facts">
          <FactRow icon={Info} label="المكونات" value={p.ingredients} />
          <FactRow icon={Scale} label="الأوزان / الأحجام" value={p.sizes} />
          <FactRow icon={ShieldCheck} label="طريقة الحفظ" value={p.storage} />
          <FactRow icon={Clock} label="تاريخ الصلاحية" value={p.expiry} />
        </div>
        <SourceNote text="المصدر: صفحة المنتج على الموقع الرسمي لمجموعة GOUMIDI." />
        <button className="btn-primary full" onClick={() => go("products")}>العودة إلى المنتجات</button>
      </div>
    </div>
  );
}

function AwardsScreen({ go, data }) {
  const cats = [
    { title: "شهادات الجودة", items: [data.company.iso] },
    { title: "الجوائز", items: [] },
    { title: "المعارض", items: data.news.map(n => `${n.title} — ${n.date}`) },
    { title: "الإنجازات", items: ["حضور على المستويين الوطني والدولي وتأسيس 3 علامات تجارية (OKID'S، BRAVO، TASTY)."] },
    { title: "المشاركات الدولية", items: ["IFSA — المعرض الدولي للصناعات الغذائية، تونس (2026)."] },
  ];
  return (
    <div className="screen">
      <TopBar title="الجوائز والإنجازات" onBack={() => go("home")} />
      <div className="content-pad">
        {cats.map((c, i) => (
          <div key={i} className="card soft" style={{ marginBottom: 14 }}>
            <div className="award-cat-title"><Award size={16} /> {c.title}</div>
            {c.items.length ? (
              <ul className="bullet-list">{c.items.map((it, j) => <li key={j}>{it}</li>)}</ul>
            ) : (
              <p className="hint no-margin">سيتم تحديث هذا القسم عند توفر معلومات رسمية.</p>
            )}
          </div>
        ))}
      </div>
    </div>
  );
}

function NewsScreen({ data, go }) {
  return (
    <div className="screen">
      <TopBar title="المعارض والأخبار" onBack={() => go("home")} />
      <div className="content-pad">
        {data.news.map(n => (
          <div key={n.id} className="news-card">
            <div className="news-card-img"><SmartImage id={n.id} folder="news" remoteSrc={n.img} alt={n.title} className="news-img" boxClassName="news-img-box" iconSize={20} /></div>
            <div className="news-card-body">
              <div className="news-card-date"><Clock size={13}/> {n.date}</div>
              <div className="news-card-title">{n.title}</div>
              <div className="news-card-place"><MapPin size={13}/> {n.place}</div>
              <p>{n.desc}</p>
              <a className="link-more" href={n.link} target="_blank" rel="noreferrer">اقرأ المزيد <ExternalLink size={14}/></a>
            </div>
          </div>
        ))}
      </div>
    </div>
  );
}

function LocationScreen({ data, go }) {
  const c = data.company;
  const mapsUrl = `https://www.google.com/maps/search/?api=1&query=${encodeURIComponent(c.address)}`;
  return (
    <div className="screen">
      <TopBar title="موقع الشركة" onBack={() => go("home")} />
      <div className="content-pad">
        <div className="map-embed">
          <iframe
            title="map"
            src={`https://maps.google.com/maps?q=${encodeURIComponent(c.address)}&z=15&output=embed`}
            loading="lazy"
          />
        </div>
        <div className="card soft">
          <InfoRow icon={MapPin} label="العنوان" value={c.address} />
          <InfoRow icon={Phone} label="الهاتف" value={c.phone} />
          <InfoRow icon={Mail} label="البريد الإلكتروني" value={c.email} />
        </div>
        <div className="cta-row">
          <a className="btn-primary" href={mapsUrl} target="_blank" rel="noreferrer">فتح Google Maps</a>
          <a className="btn-ghost" href={`tel:${c.phone.replace(/[^+\d]/g, "")}`}>اتصال</a>
        </div>
      </div>
    </div>
  );
}

function EmployeesScreen({ data, go }) {
  return (
    <div className="screen">
      <TopBar title="الموظفون" onBack={() => go("home")} />
      <div className="content-pad">
        <div className="card soft center">
          <Users size={30} color="#B5222E" />
          <div className="big-stat">{data.company.employeesRange}</div>
          <p className="hint">هذا الرقم نطاق تقريبي وليس عددًا دقيقًا، وفق المصادر العامة المتاحة (مثل LinkedIn). لا تُعرض أسماء أو بيانات شخصية للموظفين إلا إذا كانت منشورة رسميًا ومسموحًا باستخدامها.</p>
        </div>
      </div>
    </div>
  );
}

function BranchesScreen({ data, go }) {
  return (
    <div className="screen">
      <TopBar title="الشركات والفروع" onBack={() => go("home")} />
      <div className="content-pad">
        <div className="card soft">
          <div className="award-cat-title"><Factory size={16}/> فروع المجموعة</div>
          <p>{data.branches.note}</p>
        </div>
      </div>
    </div>
  );
}

function RecipesScreen({ data, go }) {
  return (
    <div className="screen">
      <TopBar title="الوصفات" onBack={() => go("home")} />
      <div className="content-pad">
        <div className="recipe-grid">
          {data.recipes.map(r => (
            <div key={r.id} className="recipe-card">
              <SmartImage id={r.id} folder="recipes" remoteSrc={r.img} alt={r.title} className="recipe-img" boxClassName="recipe-img-box" iconSize={18} />
              <div className="recipe-body">
                <div className="recipe-title">{r.title}</div>
                <div className="recipe-meta"><Clock size={13}/> {r.time} · {r.product}</div>
                <p className="hint no-margin">{r.ingredients}</p>
              </div>
            </div>
          ))}
        </div>
      </div>
    </div>
  );
}

function QualityScreen({ data, go }) {
  return (
    <div className="screen">
      <TopBar title="عن الجودة" onBack={() => go("home")} />
      <div className="content-pad">
        <div className="card soft">
          <div className="award-cat-title"><ShieldCheck size={16}/> شهادة ISO 9001</div>
          <p>حصلت الشركة على شهادة {data.company.iso}، وذلك ضمن التزامها بمعايير الجودة في تصنيع وتعبئة منتجات الألبان.</p>
        </div>
        <SourceNote text="المصدر: الموقع الرسمي لمجموعة GOUMIDI." />
      </div>
    </div>
  );
}

function ContactScreen({ data, go }) {
  const c = data.company;
  return (
    <div className="screen">
      <TopBar title="تواصل معنا" onBack={() => go("home")} />
      <div className="content-pad">
        <div className="card soft">
          <InfoRow icon={Phone} label="الهاتف" value={c.phone} />
          <InfoRow icon={Mail} label="البريد الإلكتروني" value={c.email} />
          <InfoRow icon={MapPin} label="العنوان" value={c.address} />
        </div>
        <div className="social-row">
          <a href={c.socials.instagram} target="_blank" rel="noreferrer"><Instagram size={20}/></a>
          <a href={c.socials.facebook} target="_blank" rel="noreferrer"><Facebook size={20}/></a>
          <a href={c.socials.linkedin} target="_blank" rel="noreferrer"><Linkedin size={20}/></a>
          <a href={c.socials.youtube} target="_blank" rel="noreferrer"><Youtube size={20}/></a>
        </div>
        <a className="btn-primary full" href={`https://www.google.com/maps/search/?api=1&query=${encodeURIComponent(c.address)}`} target="_blank" rel="noreferrer">فتح Google Maps</a>
      </div>
    </div>
  );
}

function FavoritesScreen({ products, favs, go, openProduct, toggleFav }) {
  const list = products.filter(p => favs.includes(p.id));
  return (
    <div className="screen">
      <TopBar title="المفضلة" onBack={() => go("home")} />
      <div className="content-pad">
        {list.length === 0 ? (
          <EmptyState text="لم تُضِف أي منتج إلى المفضلة بعد. اضغط على أيقونة القلب داخل بطاقة المنتج." />
        ) : (
          <div className="product-grid">
            {list.map(p => <ProductCard key={p.id} p={p} onOpen={openProduct} fav={true} onToggleFav={toggleFav} />)}
          </div>
        )}
      </div>
    </div>
  );
}

function CompareScreen({ products, compareIds, toggleCompareSelect, compareProducts, go }) {
  return (
    <div className="screen">
      <TopBar title="مقارنة المنتجات" onBack={() => go("home")} />
      <div className="content-pad">
        <p className="hint">اختر منتجَين للمقارنة بينهما.</p>
        <div className="product-grid">
          {products.map(p => (
            <ProductCard key={p.id} p={p} compareMode selected={compareIds.includes(p.id)} onSelect={toggleCompareSelect} onOpen={() => {}} fav={false} onToggleFav={() => {}} />
          ))}
        </div>

        {compareProducts.length === 2 && (
          <div className="compare-table-wrap">
            <table className="compare-table">
              <thead>
                <tr>
                  <th></th>
                  {compareProducts.map(p => <th key={p.id}><img src={p.img} alt={p.name} /><div>{p.name}</div></th>)}
                </tr>
              </thead>
              <tbody>
                <tr><td>العلامة</td>{compareProducts.map(p => <td key={p.id}>{p.brand}</td>)}</tr>
                <tr><td>النوع</td>{compareProducts.map(p => <td key={p.id}>{p.type}</td>)}</tr>
                <tr><td>الحجم</td>{compareProducts.map(p => <td key={p.id}>{p.sizes}</td>)}</tr>
                <tr><td>المكونات</td>{compareProducts.map(p => <td key={p.id}>{p.ingredients}</td>)}</tr>
                <tr><td>الاستخدام</td>{compareProducts.map(p => <td key={p.id}>{p.desc}</td>)}</tr>
              </tbody>
            </table>
          </div>
        )}
      </div>
    </div>
  );
}

function SourcesScreen({ data, go }) {
  return (
    <div className="screen">
      <TopBar title="المصادر والمراجع" onBack={() => go("home")} />
      <div className="content-pad">
        <p className="hint">الأولوية دائمًا للموقع الرسمي للشركة. كل معلومة مهمة في هذا التطبيق مأخوذة من أحد المصادر التالية:</p>
        <div className="card soft">
          {data.sources.map((s, i) => (
            <a key={i} className="source-row" href={s.url} target="_blank" rel="noreferrer">
              <BookMarked size={16}/> <span>{s.label}</span> <ExternalLink size={14} style={{ marginInlineStart: "auto" }}/>
            </a>
          ))}
        </div>
      </div>
    </div>
  );
}

/* ============================== Admin ============================== */
function AdminScreen({ go, data, updateData, authed, setAuthed, pass, setPass, error, setError, showToast }) {
  const [tab, setTab] = useState("company");
  const [newProduct, setNewProduct] = useState(null);
  const [editingId, setEditingId] = useState(null);
  const [newNews, setNewNews] = useState({ title: "", date: "", place: "", desc: "", link: "" });

  const login = (e) => {
    e.preventDefault();
    if (pass === "okids2026") { setAuthed(true); setError(""); }
    else setError("كلمة المرور غير صحيحة.");
  };

  if (!authed) {
    return (
      <div className="screen">
        <TopBar title="لوحة التحكم" onBack={() => go("home")} />
        <div className="content-pad">
          <div className="card soft center">
            <Lock size={26} color="#B5222E" />
            <h3 style={{ margin: "10px 0 4px" }}>دخول المدير</h3>
            <p className="hint no-margin">هذه لوحة تجريبية توضيحية لإدارة محتوى التطبيق (منتجات، أخبار، بيانات الشركة).</p>
            <form onSubmit={login} className="admin-login">
              <input type="password" placeholder="كلمة المرور" value={pass} onChange={(e) => setPass(e.target.value)} />
              <button className="btn-primary full" type="submit">دخول</button>
            </form>
            {error && <div className="error-text">{error}</div>}
            <p className="hint tiny no-margin">كلمة المرور التجريبية: okids2026 — تنبيه: هذا نموذج أولي بلا نظام دخول أو تشفير حقيقي؛ الربط بقاعدة بيانات وحسابات مدير فعلية يتطلب خادمًا خلفيًا حقيقيًا.</p>
          </div>
        </div>
      </div>
    );
  }

  const c = data.company;

  const saveCompanyField = (field, value) => updateData(d => { d.company[field] = value; return d; });

  const addProduct = () => {
    const p = newProduct;
    if (!p?.name || !p?.brand) return;
    updateData(d => { d.products.push({ ...p, id: p.name.toLowerCase().replace(/\s+/g, "-") + "-" + Date.now() }); return d; });
    setNewProduct(null);
    showToast("تمت إضافة المنتج");
  };
  const deleteProduct = (id) => updateData(d => { d.products = d.products.filter(p => p.id !== id); return d; });
  const saveEditProduct = (id, field, value) => updateData(d => { const p = d.products.find(x => x.id === id); if (p) p[field] = value; return d; });

  const addNews = () => {
    if (!newNews.title || !newNews.date) return;
    updateData(d => { d.news.unshift({ ...newNews, id: "news-" + Date.now(), img: LOGO }); return d; });
    setNewNews({ title: "", date: "", place: "", desc: "", link: "" });
    showToast("تمت إضافة الخبر");
  };
  const deleteNews = (id) => updateData(d => { d.news = d.news.filter(n => n.id !== id); return d; });

  return (
    <div className="screen">
      <TopBar title="لوحة التحكم" onBack={() => go("home")} right={
        <button className="icon-btn" onClick={() => setAuthed(false)} aria-label="خروج"><LogOut size={18}/></button>
      } />
      <div className="content-pad">
        <div className="chip-row">
          {[["company","بيانات الشركة"],["products","المنتجات"],["news","الأخبار"]].map(([id,label]) => (
            <button key={id} className={"chip" + (tab === id ? " active" : "")} onClick={() => setTab(id)}>{label}</button>
          ))}
        </div>

        {tab === "company" && (
          <div className="card soft">
            <AdminField label="عدد الموظفين (نطاق)" value={c.employeesRange} onSave={(v) => saveCompanyField("employeesRange", v)} />
            <AdminField label="العنوان" value={c.address} onSave={(v) => saveCompanyField("address", v)} />
            <AdminField label="الهاتف" value={c.phone} onSave={(v) => saveCompanyField("phone", v)} />
            <AdminField label="البريد الإلكتروني" value={c.email} onSave={(v) => saveCompanyField("email", v)} />
            <AdminField label="نص «من نحن»" value={c.about} textarea onSave={(v) => saveCompanyField("about", v)} />
          </div>
        )}

        {tab === "products" && (
          <>
            <button className="btn-primary full" onClick={() => setNewProduct({ name: "", brand: "OKID'S", type: "", desc: "", img: "", ingredients: "", sizes: "", storage: "", expiry: "" })}>
              <Plus size={16}/> إضافة منتج جديد
            </button>
            {newProduct && (
              <div className="card soft" style={{ marginTop: 10 }}>
                {["name","brand","type","desc","img","ingredients","sizes","storage","expiry"].map(f => (
                  <input key={f} className="admin-input" placeholder={f} value={newProduct[f]} onChange={(e) => setNewProduct({ ...newProduct, [f]: e.target.value })} />
                ))}
                {!newProduct.img && <p className="hint tiny no-margin"><ImageIcon size={12}/> لا توجد صورة رسمية؟ اترك الحقل فارغًا وسيظهر مكان مخصص للصورة بدل صورة مزيفة.</p>}
                <button className="btn-primary full" onClick={addProduct}>حفظ المنتج</button>
              </div>
            )}
            <div className="admin-list">
              {data.products.map(p => (
                <div key={p.id} className="admin-row">
                  <SmartImage id={p.id} remoteSrc={p.img} alt="" className="admin-thumb" boxClassName="admin-thumb-box" iconSize={14} />
                  <div className="admin-row-body">
                    {editingId === p.id ? (
                      <>
                        <input className="admin-input" value={p.name} onChange={(e) => saveEditProduct(p.id, "name", e.target.value)} />
                        <input className="admin-input" value={p.desc} onChange={(e) => saveEditProduct(p.id, "desc", e.target.value)} />
                      </>
                    ) : (
                      <>
                        <div className="admin-row-title">{p.name}</div>
                        <div className="hint tiny no-margin">{p.brand} · {p.type}</div>
                      </>
                    )}
                  </div>
                  <button className="icon-btn" onClick={() => setEditingId(editingId === p.id ? null : p.id)}><Pencil size={16}/></button>
                  <button className="icon-btn danger" onClick={() => deleteProduct(p.id)}><Trash2 size={16}/></button>
                </div>
              ))}
            </div>
          </>
        )}

        {tab === "news" && (
          <>
            <div className="card soft">
              <input className="admin-input" placeholder="عنوان الخبر" value={newNews.title} onChange={(e) => setNewNews({ ...newNews, title: e.target.value })} />
              <input className="admin-input" placeholder="التاريخ (YYYY-MM-DD)" value={newNews.date} onChange={(e) => setNewNews({ ...newNews, date: e.target.value })} />
              <input className="admin-input" placeholder="المكان" value={newNews.place} onChange={(e) => setNewNews({ ...newNews, place: e.target.value })} />
              <input className="admin-input" placeholder="وصف مختصر" value={newNews.desc} onChange={(e) => setNewNews({ ...newNews, desc: e.target.value })} />
              <button className="btn-primary full" onClick={addNews}><Plus size={16}/> إضافة خبر</button>
            </div>
            <div className="admin-list">
              {data.news.map(n => (
                <div key={n.id} className="admin-row">
                  <div className="admin-row-body">
                    <div className="admin-row-title">{n.title}</div>
                    <div className="hint tiny no-margin">{n.date} · {n.place}</div>
                  </div>
                  <button className="icon-btn danger" onClick={() => deleteNews(n.id)}><Trash2 size={16}/></button>
                </div>
              ))}
            </div>
          </>
        )}
      </div>
    </div>
  );
}

function AdminField({ label, value, onSave, textarea }) {
  const [v, setV] = useState(value);
  useEffect(() => setV(value), [value]);
  return (
    <div className="admin-field">
      <label>{label}</label>
      {textarea ? (
        <textarea className="admin-input" rows={4} value={v} onChange={(e) => setV(e.target.value)} onBlur={() => onSave(v)} />
      ) : (
        <input className="admin-input" value={v} onChange={(e) => setV(e.target.value)} onBlur={() => onSave(v)} />
      )}
    </div>
  );
}

/* ============================== Small components ============================== */
function InfoRow({ icon: Icon, label, value }) {
  return (
    <div className="info-row">
      <div className="info-row-icon"><Icon size={16} /></div>
      <div>
        <div className="info-row-label">{label}</div>
        <div className="info-row-value">{value}</div>
      </div>
    </div>
  );
}
function FactRow({ icon: Icon, label, value }) {
  return (
    <div className="fact-row">
      <Icon size={16} color="#B5222E" />
      <div>
        <div className="fact-label">{label}</div>
        <div className="fact-value">{value}</div>
      </div>
    </div>
  );
}
function SourceNote({ text }) {
  return <div className="source-note"><BookMarked size={13}/> {text}</div>;
}
function EmptyState({ text }) {
  return <div className="empty-state"><Search size={26} color="#c9c0ae" /><p>{text}</p></div>;
}

/* ============================== Styles ============================== */
function Style() {
  return (
    <style>{`
      @import url('https://fonts.googleapis.com/css2?family=El+Messiri:wght@500;600;700&family=Tajawal:wght@400;500;700;900&display=swap');

      :root{
        --ink:#241C15; --cream:#FBF6EC; --paper:#FFFFFF; --gold:#C89B3C;
        --okid:#B5222E; --bravo:#1D4E89; --tasty:#D69A22; --line:#EAE1CE;
        --muted:#8a8474;
      }
      *{box-sizing:border-box;}
      .app-shell{
        font-family:'Tajawal',sans-serif; background:var(--cream); color:var(--ink);
        min-height:100vh; display:flex; justify-content:center;
      }
      .app-frame{ width:100%; max-width:480px; min-height:100vh; background:var(--cream); position:relative; padding-bottom:78px; }
      h1,h2,h3{ font-family:'El Messiri',serif; margin:0; }
      button{ font-family:inherit; cursor:pointer; }
      input, textarea{ font-family:inherit; }
      a{ color:inherit; text-decoration:none; }

      .loading-screen{ height:100vh; display:flex; flex-direction:column; align-items:center; justify-content:center; gap:18px; }
      .spinner{ width:28px; height:28px; border-radius:50%; border:3px solid var(--line); border-top-color:var(--okid); animation:spin 0.8s linear infinite; }
      @keyframes spin{ to{ transform:rotate(360deg);} }

      /* Hero */
      .hero{ background: linear-gradient(180deg,#241C15 0%, #3a2a1c 100%); color:#fff; padding:28px 20px 34px; text-align:center; border-radius:0 0 28px 28px; position:relative; overflow:hidden; }
      .hero::after{ content:""; position:absolute; inset:0; background: radial-gradient(circle at 85% -10%, rgba(197,34,46,0.35), transparent 55%); pointer-events:none; }
      .hero-logo{ width:64px; margin-bottom:10px; filter:brightness(0) invert(1); opacity:0.92; }
      .hero-badge{ display:inline-flex; align-items:center; gap:6px; background:rgba(255,255,255,0.1); border:1px solid rgba(255,255,255,0.18); padding:5px 12px; border-radius:20px; font-size:12px; margin-bottom:12px; }
      .hero h1{ font-size:26px; line-height:1.35; margin-bottom:10px; }
      .hero h1 span{ color:#E8A23B; }
      .hero p{ font-size:13.5px; opacity:0.82; line-height:1.7; max-width:340px; margin:0 auto 18px; }
      .hero-actions{ display:flex; gap:10px; justify-content:center; margin-bottom:16px; flex-wrap:wrap; }
      .hero-links{ display:flex; gap:8px; justify-content:center; flex-wrap:wrap; }
      .hero-links button{ background:transparent; border:1px solid rgba(255,255,255,0.25); color:#fff; font-size:12px; padding:6px 12px; border-radius:16px; }

      .btn-primary{ background:var(--okid); color:#fff; border:none; padding:12px 20px; border-radius:12px; font-weight:700; font-size:14px; display:inline-flex; align-items:center; gap:6px; justify-content:center; }
      .btn-primary.full{ width:100%; margin-top:14px; }
      .btn-ghost{ background:rgba(255,255,255,0.08); color:#fff; border:1px solid rgba(255,255,255,0.3); padding:12px 20px; border-radius:12px; font-weight:700; font-size:14px; }
      .btn-outline{ background:transparent; border:1.5px solid var(--okid); color:var(--okid); border-radius:10px; font-weight:700; }
      .btn-outline.small{ padding:7px 10px; font-size:12.5px; width:100%; margin-top:8px; display:flex; align-items:center; justify-content:center; gap:4px; }

      .stats-strip{ display:grid; grid-template-columns:repeat(2,1fr); gap:10px; padding:16px 20px 4px; }
      .stat{ background:var(--paper); border:1px solid var(--line); border-radius:14px; padding:12px; text-align:center; }
      .stat-num{ display:block; font-family:'El Messiri',serif; font-weight:700; color:var(--okid); font-size:16px; }
      .stat-label{ font-size:11px; color:var(--muted); }

      .section-title{ padding:22px 20px 10px; }
      .eyebrow{ display:flex; align-items:center; gap:6px; font-size:11px; letter-spacing:1.5px; color:var(--gold); font-weight:700; text-transform:uppercase; margin-bottom:4px; }
      .dot{ width:6px; height:6px; border-radius:50%; background:var(--gold); }
      .section-title h2{ font-size:20px; }
      .section-title .sub{ font-size:12.5px; color:var(--muted); margin-top:4px; }

      .h-scroll{ display:flex; gap:12px; overflow-x:auto; padding:4px 20px 8px; scrollbar-width:none; }
      .h-scroll::-webkit-scrollbar{ display:none; }
      .mini-card{ min-width:130px; background:var(--paper); border:1px solid var(--line); border-radius:14px; overflow:hidden; flex-shrink:0; }
      .mini-band{ color:#fff; font-size:10px; font-weight:700; padding:3px 8px; }
      .mini-img, .mini-img-box{ width:100%; height:90px; object-fit:contain; background:#fff; padding:6px; display:block; }
      .mini-img-box{ display:flex; flex-direction:column; align-items:center; justify-content:center; gap:4px; color:#c9c0ae; text-align:center; }
      .mini-img-box span{ font-size:8.5px; line-height:1.3; padding:0 6px; }
      .mini-name{ font-size:12px; font-weight:700; padding:6px 8px 10px; }

      /* Smart image fallback (generic) */
      .img-fallback{ display:flex; flex-direction:column; align-items:center; justify-content:center; gap:6px; color:#b4ab97; background:var(--cream); width:100%; height:100%; text-align:center; }
      .img-fallback span{ font-size:11px; font-weight:700; line-height:1.4; padding:0 10px; }

      .link-more{ display:flex; align-items:center; gap:4px; background:none; border:none; color:var(--okid); font-weight:700; font-size:13px; padding:2px 20px 4px; }

      .news-list{ padding:0 20px; display:flex; flex-direction:column; gap:8px; }
      .news-row{ display:flex; gap:10px; background:var(--paper); border:1px solid var(--line); border-radius:12px; padding:10px 12px; }
      .news-row-date{ font-size:11px; color:var(--gold); font-weight:700; white-space:nowrap; }
      .news-row-title{ font-weight:700; font-size:13.5px; }
      .news-row-place{ display:flex; align-items:center; gap:4px; font-size:11px; color:var(--muted); margin-top:2px; }

      .bottom-spacer{ height:20px; }

      /* Topbar */
      .topbar{ display:flex; align-items:center; gap:10px; padding:16px 16px 12px; background:var(--cream); position:sticky; top:0; z-index:5; }
      .topbar h1{ font-size:17px; flex:1; }
      .topbar-logo{ width:30px; }
      .topbar-right{ min-width:20px; }
      .icon-btn{ background:var(--paper); border:1px solid var(--line); width:36px; height:36px; border-radius:10px; display:flex; align-items:center; justify-content:center; }
      .icon-btn.danger{ color:#c0392b; }

      .content-pad{ padding:0 18px 30px; }
      .card.soft{ background:var(--paper); border:1px solid var(--line); border-radius:16px; padding:16px; }
      .card.center{ text-align:center; }
      .lead{ font-size:14px; line-height:2; margin:0; }

      .info-grid{ display:flex; flex-direction:column; gap:10px; margin-top:14px; }
      .info-row{ display:flex; gap:10px; background:var(--paper); border:1px solid var(--line); border-radius:12px; padding:10px 12px; align-items:flex-start; }
      .info-row-icon{ width:32px; height:32px; border-radius:9px; background:var(--cream); display:flex; align-items:center; justify-content:center; color:var(--okid); flex-shrink:0; }
      .info-row-label{ font-size:11px; color:var(--muted); }
      .info-row-value{ font-size:13.5px; font-weight:700; }

      .source-note{ display:flex; align-items:center; gap:6px; font-size:11.5px; color:var(--muted); margin-top:12px; }
      .hint{ font-size:12.5px; color:var(--muted); line-height:1.8; margin-top:10px; }
      .hint.no-margin{ margin-top:6px; }
      .hint.tiny{ font-size:11px; }

      /* Timeline */
      .timeline{ position:relative; padding-inline-start:18px; border-inline-start:2px dashed var(--line); margin-top:8px; }
      .tl-item{ position:relative; padding-bottom:22px; padding-inline-start:16px; }
      .tl-dot{ position:absolute; inline-size:12px; block-size:12px; border-radius:50%; background:var(--okid); inset-inline-start:-25px; top:4px; border:2px solid var(--cream); }
      .tl-year{ font-family:'El Messiri',serif; color:var(--okid); font-weight:700; font-size:15px; margin-bottom:4px; }
      .tl-card{ background:var(--paper); border:1px solid var(--line); border-radius:12px; padding:12px; }
      .tl-title{ font-weight:700; margin-bottom:4px; font-size:13.5px; }
      .tl-card p{ font-size:12.5px; color:var(--muted); margin:0; line-height:1.7; }

      /* Search & chips */
      .search-box{ display:flex; align-items:center; gap:8px; background:var(--paper); border:1px solid var(--line); border-radius:12px; padding:10px 14px; margin:12px 0; }
      .search-box input{ border:none; outline:none; background:transparent; font-size:13.5px; flex:1; color:var(--ink); }
      .chip-row{ display:flex; gap:8px; overflow-x:auto; padding-bottom:10px; }
      .chip{ background:var(--paper); border:1.5px solid var(--line); padding:7px 14px; border-radius:20px; font-size:12.5px; font-weight:700; white-space:nowrap; }
      .chip.active{ background:var(--ink); color:#fff; border-color:var(--ink); }

      /* Product grid/card */
      .product-grid{ display:grid; grid-template-columns:1fr 1fr; gap:12px; }
      .product-card{ background:var(--paper); border:2px solid transparent; border-radius:16px; padding:10px; position:relative; box-shadow:0 2px 10px rgba(36,28,21,0.05); }
      .product-band{ position:absolute; top:10px; right:10px; color:#fff; font-size:9px; font-weight:700; padding:3px 8px; border-radius:6px; z-index:2; }
      .fav-btn{ position:absolute; top:8px; left:8px; background:#fff; border:1px solid var(--line); width:28px; height:28px; border-radius:50%; display:flex; align-items:center; justify-content:center; z-index:2; }
      .product-img-wrap{ background:var(--cream); border-radius:12px; height:110px; display:flex; align-items:center; justify-content:center; overflow:hidden; margin-top:6px; cursor:pointer; }
      .prod-img{ max-width:88%; max-height:88%; width:auto; height:auto; object-fit:contain; }
      .prod-img-box{ background:transparent; }
      .prod-img-box span{ font-size:10px; }
      .product-body{ padding:10px 2px 0; }
      .product-type{ font-size:10.5px; color:var(--muted); }
      .product-name{ font-weight:700; font-size:13.5px; margin:2px 0; }
      .product-desc{ font-size:11px; color:var(--muted); line-height:1.5; min-height:32px; }

      .empty-state{ text-align:center; padding:40px 20px; color:var(--muted); }
      .empty-state p{ font-size:13px; margin-top:8px; }

      /* Product detail */
      .pd-hero{ height:220px; display:flex; align-items:center; justify-content:center; position:relative; }
      .pd-hero-img{ max-height:82%; max-width:70%; width:auto; height:auto; object-fit:contain; cursor:zoom-in; }
      .pd-hero-fallback{ width:70%; height:82%; cursor:default; }
      .pd-hero-hint{ position:absolute; bottom:10px; left:50%; transform:translateX(-50%); background:rgba(36,28,21,0.55); color:#fff; font-size:10.5px; padding:4px 10px; border-radius:20px; display:flex; align-items:center; gap:4px; pointer-events:none; }
      .lightbox-backdrop{ position:fixed; inset:0; background:rgba(15,11,7,0.92); z-index:80; display:flex; align-items:center; justify-content:center; padding:30px 20px; }
      .lightbox-img{ max-width:100%; max-height:80vh; object-fit:contain; }
      .lightbox-fallback{ width:260px; height:260px; border-radius:16px; }
      .lightbox-close{ position:absolute; top:20px; left:20px; background:rgba(255,255,255,0.12); border:1px solid rgba(255,255,255,0.3); color:#fff; width:38px; height:38px; border-radius:50%; display:flex; align-items:center; justify-content:center; }
      .pd-head{ display:flex; justify-content:space-between; align-items:center; margin:14px 0 6px; }
      .pill{ font-size:11px; font-weight:700; padding:4px 12px; border-radius:20px; }
      .pd-title{ font-size:21px; margin-top:8px; }
      .pd-type{ color:var(--muted); font-size:13px; margin:2px 0 10px; }
      .pd-desc{ font-size:13.5px; line-height:1.8; }
      .pd-facts{ display:flex; flex-direction:column; gap:10px; margin-top:14px; }
      .fact-row{ display:flex; gap:10px; background:var(--paper); border:1px solid var(--line); padding:12px; border-radius:12px; }
      .fact-label{ font-size:11px; color:var(--muted); }
      .fact-value{ font-size:13px; font-weight:700; margin-top:2px; }

      /* Awards */
      .award-cat-title{ display:flex; align-items:center; gap:6px; font-weight:700; margin-bottom:8px; font-size:14px; }
      .bullet-list{ margin:0; padding-inline-start:18px; font-size:13px; color:var(--ink); line-height:2; }

      /* News cards */
      .news-card{ background:var(--paper); border:1px solid var(--line); border-radius:16px; overflow:hidden; margin-bottom:14px; }
      .news-card-img{ height:120px; background:var(--cream); display:flex; align-items:center; justify-content:center; overflow:hidden; }
      .news-img{ max-height:100%; max-width:100%; width:auto; height:auto; object-fit:contain; }
      .news-img-box span{ font-size:10px; }
      .news-card-body{ padding:14px; }
      .news-card-date{ display:flex; align-items:center; gap:5px; font-size:11px; color:var(--gold); font-weight:700; }
      .news-card-title{ font-family:'El Messiri',serif; font-size:16px; margin:4px 0; }
      .news-card-place{ display:flex; align-items:center; gap:4px; font-size:11.5px; color:var(--muted); margin-bottom:8px; }
      .news-card-body p{ font-size:13px; line-height:1.8; margin:0 0 10px; }

      /* Map */
      .map-embed{ border-radius:14px; overflow:hidden; height:190px; border:1px solid var(--line); margin-bottom:14px; }
      .map-embed iframe{ width:100%; height:100%; border:0; }
      .cta-row{ display:flex; gap:10px; margin-top:14px; }
      .cta-row a{ flex:1; text-align:center; }

      .big-stat{ font-family:'El Messiri',serif; font-size:22px; color:var(--okid); font-weight:700; margin:6px 0; }

      /* Recipes */
      .recipe-grid{ display:flex; flex-direction:column; gap:12px; }
      .recipe-card{ background:var(--paper); border:1px solid var(--line); border-radius:16px; overflow:hidden; display:flex; }
      .recipe-img{ width:100px; height:100px; object-fit:cover; flex-shrink:0; }
      .recipe-img-box{ width:100px; height:100px; flex-shrink:0; padding:4px; }
      .recipe-img-box span{ font-size:9px; }
      .recipe-body{ padding:10px 12px; flex:1; }
      .recipe-title{ font-weight:700; font-size:14px; font-family:'El Messiri',serif; }
      .recipe-meta{ display:flex; align-items:center; gap:5px; font-size:11px; color:var(--muted); margin:4px 0 6px; }

      .social-row{ display:flex; gap:10px; margin:14px 0; }
      .social-row a{ width:40px; height:40px; border-radius:12px; background:var(--paper); border:1px solid var(--line); display:flex; align-items:center; justify-content:center; }

      .source-row{ display:flex; align-items:center; gap:8px; padding:10px 0; border-bottom:1px solid var(--line); font-size:13px; }
      .source-row:last-child{ border-bottom:none; }

      /* Compare */
      .compare-table-wrap{ overflow-x:auto; margin-top:18px; }
      .compare-table{ width:100%; border-collapse:collapse; background:var(--paper); border-radius:12px; overflow:hidden; font-size:12px; }
      .compare-table th, .compare-table td{ border:1px solid var(--line); padding:8px; text-align:center; }
      .compare-table th img{ width:50px; height:50px; object-fit:contain; display:block; margin:0 auto 4px; }
      .compare-table td:first-child{ font-weight:700; background:var(--cream); text-align:start; }

      /* Admin */
      .admin-login{ display:flex; flex-direction:column; gap:10px; margin-top:14px; }
      .admin-login input{ border:1px solid var(--line); border-radius:10px; padding:11px 14px; font-size:13.5px; }
      .error-text{ color:#c0392b; font-size:12.5px; margin-top:8px; }
      .admin-input{ width:100%; border:1px solid var(--line); border-radius:10px; padding:10px 12px; font-size:13px; margin-bottom:8px; background:var(--cream); }
      .admin-field{ margin-bottom:12px; }
      .admin-field label{ font-size:11.5px; color:var(--muted); display:block; margin-bottom:4px; }
      .admin-list{ display:flex; flex-direction:column; gap:8px; margin-top:14px; }
      .admin-row{ display:flex; align-items:center; gap:10px; background:var(--paper); border:1px solid var(--line); border-radius:12px; padding:8px; }
      .admin-thumb{ width:40px; height:40px; object-fit:contain; background:var(--cream); border-radius:8px; flex-shrink:0; }
      .admin-thumb-box{ width:40px; height:40px; border-radius:8px; flex-shrink:0; padding:2px; }
      .admin-thumb-box span{ display:none; }
      .admin-row-body{ flex:1; min-width:0; }
      .admin-row-title{ font-weight:700; font-size:13px; }

      /* Sheet */
      .sheet-backdrop{ position:fixed; inset:0; background:rgba(36,28,21,0.5); z-index:40; display:flex; align-items:flex-end; justify-content:center; }
      .sheet{ background:var(--cream); width:100%; max-width:480px; border-radius:22px 22px 0 0; padding:10px 18px 24px; animation:slideUp .25s ease; }
      @keyframes slideUp{ from{ transform:translateY(100%);} to{ transform:translateY(0);} }
      .sheet-handle{ width:40px; height:4px; background:var(--line); border-radius:4px; margin:6px auto 14px; }
      .sheet-title{ font-family:'El Messiri',serif; font-size:16px; margin-bottom:12px; }
      .sheet-grid{ display:grid; grid-template-columns:1fr 1fr; gap:10px; }
      .sheet-item{ display:flex; flex-direction:column; align-items:center; gap:6px; background:var(--paper); border:1px solid var(--line); border-radius:14px; padding:14px 6px; font-size:12px; font-weight:700; color:var(--ink); }
      .sheet-item svg{ color:var(--okid); }

      /* Bottom nav */
      .bottom-nav{ position:fixed; bottom:0; left:50%; transform:translateX(-50%); width:100%; max-width:480px; background:var(--paper); border-top:1px solid var(--line); display:flex; z-index:30; padding:6px 4px calc(6px + env(safe-area-inset-bottom)); }
      .nav-btn{ flex:1; background:none; border:none; display:flex; flex-direction:column; align-items:center; gap:3px; padding:6px 2px; color:var(--muted); font-size:10px; font-weight:700; border-radius:10px; }
      .nav-btn.active{ color:var(--okid); }

      .toast{ position:fixed; bottom:90px; left:50%; transform:translateX(-50%); background:var(--ink); color:#fff; padding:10px 18px; border-radius:20px; font-size:12.5px; z-index:60; }

      @media (min-width:481px){
        .app-shell{ padding:24px 0; }
        .app-frame{ border-radius:28px; box-shadow:0 20px 60px rgba(36,28,21,0.18); min-height:auto; overflow:hidden; }
        .bottom-nav{ border-radius:0 0 28px 28px; }
      }
    `}</style>
  );
}
