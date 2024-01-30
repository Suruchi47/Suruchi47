- 👋 Hi, I’m @Suruchi47
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Suruchi47/Suruchi47 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import axios from 'axios';
import Head from 'next/head';

const Home = ({ memes }) => {
  return (
    <div>
      <Head>
        <title>Reddit Memes</title>
        <meta name="description" content="A collection of memes from Reddit" />
      </Head>

      <h1>Reddit Memes</h1>

      <div>
        {memes.map((meme, index) => (
          <div key={index} className="meme-card">
            <img src={meme.url} alt={`Meme ${index + 1}`} />
          </div>
        ))}
      </div>
