- 👋 Hi, I’m @yantonovadwi
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
yantonovadwi/yantonovadwi is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
const speedtest = require('speedtest-net');

speedtest()
  .on('testing', () => {
    console.log('Testing...');
  })
  .on('results', (results) => {
    console.log(`Download speed: ${results.downloadSpeed} Mbps`);
    console.log(`Upload speed: ${results.uploadSpeed} Mbps`);
    console.log(`Ping: ${results.ping} ms`);
  })
  .on('error', (error) => {
    console.log('Error:', error);
  });
