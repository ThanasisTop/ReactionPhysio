# Reaction Physio — Link Page

Custom link page για το φυσιοθεραπευτήριο **Reaction Physio**, εναλλακτική του Linktree με πλήρη έλεγχο στο design.

## Περιεχόμενα

- Σύνδεσμοι Instagram & Facebook
- Carousel φωτογραφιών χώρου (3 ανά σελίδα, swipe υποστήριξη)
- Lightbox προβολή φωτογραφιών σε πλήρες μέγεθος
- Σύνδεσμος Google Maps
- Κουμπί τηλεφώνου (click-to-call)

## Δομή αρχείων

```
├── index.html       # Η κύρια σελίδα
├── photo1.jpg       # Φωτογραφίες χώρου (όσες θέλεις)
├── photo2.jpg
├── photo3.jpg
└── ...
```

## Πώς να προσαρμόσεις

### 1. Social links
Άνοιξε το `index.html` και βρες τα παρακάτω σημεία:

```html
<!-- Instagram -->
<a href="https://instagram.com/ΒΑΛΕ_ΤΟ_USERNAME_ΣΟΥ" ...>

<!-- Facebook -->
<a href="https://facebook.com/ΒΑΛΕ_ΤΟ_LINK_ΣΟΥ" ...>
```

### 2. Φωτογραφίες
Βάλε τα αρχεία σου στον ίδιο φάκελο με το `index.html` και αντικατέστησε τα `src` στο carousel:

```html
<div class="carousel-slide">
  <img src="photo1.jpg" alt="Χώρος 1">
</div>
```

Για να προσθέσεις περισσότερες φωτογραφίες, αντέγραψε ένα `<div class="carousel-slide">` block.

### 3. Logo
Αντικατέστησε το `RP` στο avatar με την εικόνα σου:

```html
<!-- Από: -->
<div class="avatar">RP</div>

<!-- Σε: -->
<div class="avatar"><img src="logo.jpg" alt="Reaction Physio"></div>
```

### 4. Τηλέφωνο & Google Maps

```html
<a href="tel:+306900000000">         <!-- αριθμός τηλεφώνου -->
<a href="https://maps.google.com/?q=ΔΙΕΥΘΥΝΣΗ">  <!-- διεύθυνση -->
```

## Deploy

### Netlify Drop (πιο εύκολο — χωρίς εγγραφή)
1. Πας στο [app.netlify.com/drop](https://app.netlify.com/drop)
2. Σέρνεις τον φάκελο με τα αρχεία
3. Παίρνεις άμεσα live URL

### GitHub Pages
1. Δημιουργείς repository στο GitHub
2. Ανεβάζεις τα αρχεία
3. Settings → Pages → Branch: `main` → Save
4. Το URL είναι της μορφής `username.github.io/repository-name`

## Τεχνολογίες

- Vanilla HTML / CSS / JavaScript — χωρίς εξαρτήσεις
- Χωρίς frameworks, χωρίς build step
- Πλήρως responsive για κινητά
