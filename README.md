# Πρότυπη Εφαρμογή Αδειών Στελεχών Περιφέρειας

Η παρούσα εφαρμογή αποτελεί μια πρότυπη υλοποίηση για τις ανάγκες υποβολής αιτημάτων αδείας απο τα στελέχη της Περιφέρειας. Είναι ηλεκτρονικοποημένη εσωτερική διαδικασία με την οποία αφενός οι υπάλληλοι μπορούν να υποβάλλουν το αίτημά τους για τη χορήγηση μιας άδειας και αφετέρου οι προϊστάμενοι τους μπορούν να εγκρίνουν (επίσης ηλεκτρονικά) την αποδοχή η μή της άδειας.

Η διαδικασία εκτελείτα αξιοποιώντας τα παρακάτω modules που διαθέτει η εφαρμογή. 

**Αυθεντικοποίηση Χρηστών**
Οι χρήστες συνδέονται μέσω της κεντρικής υποδομής καταλόγου (LDAP) που έχει στηθεί στην Περιφέρεια. Η υπηρεσία καταλόγου περιέχει το σύνολο των στελεχών της Περιφέρειας. Κατ αυτόν τον τρόπο ο κάθε χρήστης έχει ένα ενιαίο username και password για τη διασύνδεσή τους στις εφαρμογές της Περιφέρειας.

**Υποβολή Αίτησης**
Κατά τη σύνδεση του χρήστη μέσω του LDAP επιστρέφονται πλήθος προσωπικών του στοιχείων τα οποία αξιοποιούνται απο την εφαρμογή (Όνομα, Επίθετο, Βαθμίδα, eMail, Τμήμα κλπ). Ο χρήστης αφού συνδεθεί καλείται να συμπληρώσει τις ημερομηνίες έναρξης και λήξης καθώς και τις ημέρες (σύνολο) της αιτούμενης άδειας. Κατά την υποβολή αυτών των στοιχείων ενημερώνεται ο άμεσα προϊστάμενος του (και υπεύθυνος για την έγκριση της αίτησης) μέσω ηλ. ταχυδρομείου.

Με ανάλογο τρόπο μπορεί να υλοποιηθεί πλήθος άλλων διαδικασιών αιτήσεων απο μέρους των Υπαλλήλων της Περιφέρειας.

**Έγκρισης Αίτησης**
Ο έκαστος προϊστάμενως συνδέεται μέσω του LDAP όπως ολα τα στελέχη και πέραν της παραπάνω αίτησης έχει στη διάθεσή του επιπλέον περιβάλλον διαχείρισης για την έγκριση (ή απόρριψη) των αιτήσεων των υφιστάμενών του. Κατά τη επεξεργασία μιας αίτησης ο αιτών λαμβάνει αντίστοιχο ενημερωτικό μήνυμα στο email του.

Με ανάλογο τρόπο μπορεί να υλοποιηθεί πλήθος άλλων διαδικασιών διεκπεραίωσης αιτήσεων απο μέρους των Υπαλλήλων και στελεχών της Περιφέρειας.

**Στατιστικά Αιτήσεων**
Ένας η περισσότεροι χρήστες αποκτούν πρόσβαση σε σελίδα αποτελεσμάτων όπου περιλαμβάνονται τα στατιστικά των αδειών των στελεχών.

Οι παραπάνω διαδικασίες αξιοποιούν λειτουργικότητα η οποία διατίθεται μέσω της εφαρμογής και αποτυπώνεται στα ακόλουθα modules.

**Ενημέρωση Χρηστών**
Οι χρήστες ενημερώνονται με χρήση ηλεκτρονικού ταχυδρομείου (και μελλοντικά μέσω sms). Η εφαρμογή αξιοποιώντας τον mail server της Περιφέρειας αποστέλλει μηνύματα απλού κειμένου στους εμπλεκόμενους στη διαδικασία. Η λειτουργικότητα διατίθεται σε όλες τις εφαρμογές που θα υλοποιηθούν στο μέλλον.

**Επικοινωνία με Τρίτα Συστήματα**
Οι εφαρμογές αξιοποιούν Web Services για επικοινωνία και άντληση στοιχείων με τρίτα συστήματα και οντότητες. Τέτοια οντότητα είναι η υπηρεσία αυθεντικοποίησης των πολιτών μέσω του oAuth της ΓΓΔΕ. Επιπλέον υπηρεσίες μπορεί να είναι η Αστυνομία, το Δημοτολόγιο κλπ. Παράλληλα η εφαρμογή επικοινωνεί με χρήση Middleware διαλειτουργικότητας πέραν των παραπάνω και με εσωτερικά συστήματα στην ίδια την Περιφέρεια.

Περισσότερες πληροφορίες στο [wiki](https://github.com/eellak/opengov_adeies/wiki/%CE%95%CF%86%CE%B1%CF%81%CE%BC%CE%BF%CE%B3%CE%AE-%CE%B4%CE%B9%CE%B1%CF%87%CE%B5%CE%AF%CF%81%CE%B9%CF%83%CE%B7%CF%82-%CE%B1%CE%B4%CE%B5%CE%B9%CF%8E%CE%BD-%CF%84%CE%B7%CF%82-%CE%A0%CE%94%CE%9C) 
