- 👋 Hi, I’m Nguyễn Như Ý
- 👀 I’m interested in fullstack deverloper.
- 🌱 I’m currently learning Hanoi University of Natural Resources and Environment
- 💞️ I am looking to intern front end
- 📫 How to reach me email: nguyennhuy170400@gmail.com or khanhandli@gmail.com or phone: 0328849286
- Use Case JS
- number format() = const value = numberWithCommas(22000000) -> 22,200,000
- const numberWithCommas = (number) => {return number.toString().replace(/\B(?=(\d{3})+(?!\d))/g,",");}
-----------------------------------------------------------------------
-number format() = const value = compactNumber(22000000) -> 22M
- const compactNumber = (value) => {
  const suffixes = ["", "k", "m", "b", "t"];
  const suffixNum = Math.floor((""+value).length / 3);
  let shortValue = parseFloat((suffixNum !== 0 ? (value / Math.pow(1000, suffixNum)) : value).toPrecision(2));
  if(shortValue % 1 !== 0) {
    shortValue = shortValue.toFixed(1);
  }
  return shortValue+suffixes[suffixNum];
}


<!---
khanhandli/khanhandli is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
