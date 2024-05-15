# SI_2024_lab2_203210
Милан Бошковски 203210

Control Flow Graph
![LAB drawio](https://github.com/milanboshkovski/SI_2024_lab2_203210/assets/164159886/582db3e4-d99b-4866-b08f-69f777fbde81)
A: if (allItems == null){
B: throw new RuntimeException("allItems list can't be null!");
C: for (int i = 0; i < allItems.size(); i++)
D: Item item = allItems.get(i);
E: if (item.getName() == null || item.getName().length() == 0)
F: item.setName("unknown");
G: if (item.getBarcode() != null)
H: throw new RuntimeException("No barcode!");
I: for (int j = 0; j < item.getBarcode().length(); j++)
J: if (allowed.indexOf(c) == -1)
K: throw new RuntimeException("Invalid character in item barcode!");
L: if (item.getDiscount() > 0)
M: sum += item.getPrice()*item.getDiscount();
N: sum += item.getPrice();
O: if (item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0')
P: sum -= 30;
Q: if (sum <= payment)
R: return true;
S: return false;
