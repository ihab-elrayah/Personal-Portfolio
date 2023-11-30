<script>
export default {
  data() {
    return {
      activeTab: 1,
      tech: [
        {
          id: 1,
          name: 'Javascript',
          imageUrl: 'https://static.vecteezy.com/system/resources/previews/027/127/463/original/javascript-logo-javascript-icon-transparent-free-png.png',
          status: 'Advance'
        },
        {
          id: 2,
          name: 'Java',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/5968/5968282.png',
          status: 'Intermediate'
        },
        {
          id: 3,
          name: 'Python',
          imageUrl: 'https://cdn.freebiesupply.com/logos/large/2x/python-5-logo-png-transparent.png',
          status: 'Intermediate'
        },
        {
          id: 4,
          name: 'C++',
          imageUrl: 'https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/ISO_C%2B%2B_Logo.svg/911px-ISO_C%2B%2B_Logo.svg.png',
          status: 'Beginner'
        },
        {
          id: 5,
          name: 'NodeJS',
          imageUrl: 'https://cdn.iconscout.com/icon/free/png-256/free-node-js-1174925.png',
          status: 'Advanced'
        },
        {
          id: 6,
          name: 'ReactJS',
          imageUrl: 'https://cdn4.iconfinder.com/data/icons/logos-3/600/React.js_logo-512.png',
          status: 'Intermediate'
        },
        {
          id: 7,
          name: 'ExpressJS',
          imageUrl: 'https://upload.wikimedia.org/wikipedia/commons/thumb/b/bf/Status_iucn_EX_icon_blank.svg/2048px-Status_iucn_EX_icon_blank.svg.png',
          status: 'Intermediate'
        },
        {
          id: 8,
          name: 'Spring Boot',
          imageUrl: 'https://vscjava.gallerycdn.vsassets.io/extensions/vscjava/vscode-spring-initializr/0.11.2023070103/1688180724473/Microsoft.VisualStudio.Services.Icons.Default',
          status: 'Beginner'
        },
        {
          id: 9,
          name: 'HTML',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/1051/1051277.png',
          status: 'Advanced'
        },
        {
          id: 10,
          name: 'CSS',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/732/732190.png',
          status: 'Advanced'
        },
        {
          id: 11,
          name: 'VueJS',
          imageUrl: 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/95/Vue.js_Logo_2.svg/1200px-Vue.js_Logo_2.svg.png',
          status: 'Beginner'
        },
        {
          id: 12,
          name: 'Tailwind',
          imageUrl: 'https://upload.wikimedia.org/wikipedia/commons/d/d5/Tailwind_CSS_Logo.svg',
          status: 'Beginner'
        }
      ],
      tools: [
      {
          id: 1,
          name: 'Firebase',
          imageUrl: 'https://cdn4.iconfinder.com/data/icons/google-i-o-2016/512/google_firebase-2-512.png',
          status: 'Database'
        },
        {
          id: 2,
          name: 'MySQL',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/5968/5968313.png',
          status: 'Database'
        },
        {
          id: 3,
          name: 'PostgreSQL',
          imageUrl: 'https://cdn-icons-png.flaticon.com/512/5968/5968342.png',
          status: 'Database'
        },
        {
          id: 4,
          name: 'MongoDB',
          imageUrl: 'https://static-00.iconduck.com/assets.00/database-mongo-db-icon-1954x2048-wrw32e9l.png',
          status: 'Database'
        },
        {
          id: 5,
          name: 'Amazon Web Services',
          imageUrl: 'https://upload.wikimedia.org/wikipedia/commons/thumb/5/5c/AWS_Simple_Icons_AWS_Cloud.svg/1024px-AWS_Simple_Icons_AWS_Cloud.svg.png',
          status: 'Cloud Computing Services'
        },
        {
          id: 6,
          name: 'Google Cloud Platform',
          imageUrl: 'https://static-00.iconduck.com/assets.00/google-cloud-platform-icon-1024x823-mrdn81d1.png',
          status: 'Cloud Computing Services'
        },
        {
          id: 7,
          name: 'Git',
          imageUrl: 'https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png',
          status: 'Version Control'
        },
        {
          id: 8,
          name: 'GitHub',
          imageUrl: 'https://static-00.iconduck.com/assets.00/github-icon-2048x1988-jzvzcf2t.png',
          status: 'Git Hosting'
        },
    
      ]
    };
  }
}
</script>
<template>
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5">
    <article data-page="about">

      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          About Me &nbsp;
          <div class="h-[1px] w-32 bg-amber-200 md:w-96 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
        </div>
      </header>

      <section
        class="text-sm md:text-lg text-justify flex flex-col gap-4 md:flex-row md:gap-8 md:justify-left md:items-center">
        <div class="flex justify-center">
          <img class="w-9/12 rounded-full mb-3 fadein-up"
            src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAoHCAkPDRISEgkKCQkKDwwJCQoKCB8JCggMJSEnJyUhJCQpLi4zKSw4LSQkNDo0OD0xN0M/KDE7QDszPy40NTEBDAwMDw8QGA8QGDEdGB0xMT80PzQxNDE/PzQ0NDE0MTQ0MTQxMTExMTExNDE0PzExNDExMTExMTExMTExMTE0Mf/AABEIAMgAyAMBIgACEQEDEQH/xAAbAAABBQEBAAAAAAAAAAAAAAAFAAIDBAYBB//EADwQAAIBAgMEBwYEBgMAAwAAAAECAAMRBCExBRJBcSIyUWFygbETIzORocEGQmKCJFJz0eHwFDTxQ1NU/8QAGQEAAwEBAQAAAAAAAAAAAAAAAQIDAAQF/8QAHxEAAgMBAAMBAQEAAAAAAAAAAAECETEhAxJBUSIy/9oADAMBAAIRAxEAPwDEbNf3l+J1mipi41mY2W3vBNLT5yDVF27JFXWQOLtpLC62kVZLGYBERl8oTpr1f2wYdIQWpu+zFr7xUcpkBmhRjYeU6xnUI3RlwEYde6I9HR0C+kr7QIFBwT+U2uZK9REUsTuqoJJtewmX2r+IsO6VKa0yxI3Ufe3lvGirAwY7DLMajjC2GxWA3T7SpUTdsOgL5TImq1j2Xuc9I3fJ/NYHPWO42KnR6PsqlgFpE065FOqd73h3GvG4nY1FVdxWqsRdxd7reedCvUAtvEroLnSW12xjwu6MXUCWC7u/cbsR+PtpjqaxmvrAjBP8zBeESzA96yHCbWPsGp1K61TVCmmVWzUz2GXaKgBTqDukEZgydOOhVPAzUphbd+cD4kdPyIhzE6LyzgXEjpfO80X0MsFgPir5iHFGX1gLBm1VOcO3m8mmhh0ekqbV+Ev9WkfrLg1lbag90O6pSP1iR1BlhVtnAW0R7x/KHjrAe0x7xvKdZzmH2p/2H5r6Cdi2t/2H/b6CKUEDWzD70TWUU4/OZHZx96s11BsvSRlpVD1OfpIqzG8la4N+HGQ1mzihGAS86i1M/qW0prCNRegnNY0QMPU+qOQkfnlqe4SakBuDkJHW9mqMWUsoUlgBckSb0dGT2t+IKL71NUZqdmQ3yDt2zIsTnbiSZb2qaf8AyHNNdym7F0F72WUg0tFUTkzgAtnrziLC3LOdCMdFLX1CjeMf/wATE/8A56vd7s5zWv0Hq3hHf+57Zw2kj4asouaVQDTNLWkHGFNM1NaSi4GsLbJx+5dHd2TI01tvFWvA1zadVyD3ixglG+GjKmeo1SHpU2GauqsuWe7A+IGZPlO7E2nVrUQj0wPZBVpsBZXWPxKZN5GQUadHRJpq0V8J8VOdoctAeF+KnO0OX/tB5NBDBwN+eZkG0s6P76XrJ0BkWPzonxU/WJHUGWFM6wJtT4jeRhtjnAm1fiN+2dZzmI2t/wBh/wBvoIp3a/x25J6TsosFCuzbe2XnNYhUTI4A+9XnNci5X46yMtHjhYXPWV3Wzd3CTobiRVRnFHIyftClb4a/tMFDWFq/w17t2GP0Vhyhmg8IkbNYEHMG4MfQ6g8IjGUxGOjzDa9FaeIdQSQGY6btpFs7C+2rKh6nWfwzZ/iPYxxC79Owr0weju/EX+8z/wCHqLrXqAqVemFUgizA3jSlUG1poxuaRrNn7PwyKLU0W2mWZlmqgI05ZTmHHRzPLOSOV4nLnPOXs3bPQ/lcQMxGHXsv25Xme2rs+mVLBd11uRYWuZp8SU/+xMtelBWLsw1uGyBBuDOiDlFkZqMlRiTfz0M7aT46nuORwvIaaFmAAuWIE7k7VnA1To0/4UqVOkLXXok3GQEM4k5NyBkWxMI9Gjus4O8SaaW6iyTEg9KRbuRWqiV8N108UNiA6B6aeMQ4v9hE8mhgSLIMZ8Fuan6yc/2kGOt7Fv2n6xY6hpYUjrAu1R7w8lho6wNtT4h5LOo5zE7Y+OfCs7Ftr/sHwrFKIUJYA++XnabCkcrfKY3B/FXmJsaenykZFEPS4MVf6x9jfKR1h84gxEozhV1LUl8jBUL026A5CNEVhfDmyLnqAI5rdsgpN0RlfKMZ7DL/AMisdDq7qogHa+m+rezOlR6ae8deyEqjuTnpG06aOVB4sd7vW0hKdIt442zMPVq7wKNihYBrs3RIhqu1U4VXO8pYgdjCEsTgcImYW76AXvnHY1P4ZVAzGZHG8m/KnVIuvHV2zIKliWNBq2+xUDf6Sd8lRFNyEqUrXDU3zUw7hcLSYdIDfGRGhkG0cPTQZZajXWVfkvlE1CugPC7Op4io5cXWmOiL23mlTB4VKdWoSfhby0x2Zw3sl91KjWz3rlrZKsFVHBNRhq+8T35y0ZPCE4rTV4c3pof0qZDi7brd+k7hG92nhWRYs6/KBaB4VMP117LiHVGUBUR018S8YdXSDyGgPYXA+shx+VB+4KfrJyJX2if4ep4fvJx0eWFQ6wLtUe8PhWGoH2r8Q+FZ1nMYrbfx/wBi/eKd258ceAepilFgrL2F+IvMTZ4cZDkII2j+Hq2ErlSWPs2utxZaqdohekbKPKQk0ysU0TCQ1Dnfyk4F5FWSKEihBHtTHlB7ZS2nwxGiCQZw92QdlhJKiALkM4sJ8Ne2wjmIb0iS+jRBzk3OUru7IL20IOugluqtjKtdTukW4G052rdMvF10jo4vecmpUVbiyIzWMa/tLbod3p5sMjvLIsFUpVEzRaj02vp0gRCY2sVXdDOpsVzp7zW5zRSvpa248B1SoEAvU9m+qn8zGQYqpUZc+y575ZqHeYu5LuclLm5WDsXVJFhqchHrvCcmUqeKqrTdBu7jk3O70gJX/Kw/SZYrYSoiK26Xp1Ad0qL2YSPDIC1iMjcS6VHNJ2zS4O/sk8KyHGN6y1QACL2boEq4z7xFoXhVpHpr4lh5D/aAE6y+JYfT/M3lNAfvSvtI/wANU8F/OTqDY/SQbRH8NU8BMlHR5YVL/aCNrHp/tWFhoOQgna/xP2rOw5jGbb+MPAPUxTu3PjDwD1MUosFPT/xbiva41lBulALRXsLcfrAiuwNgTkBfsvH1KmZdmJZyScrlmkaZ3JXd3jexNyBOU66J0r1F437iI84je1S3bnII6C2FxTJC4MuUhdIMY2/9jUx7pkOkvYY8WSnH8NfhgBSGedu2OwzZ255yhsfG0K67u9uVFGdMnMjuhFKNjkdMx3wPTLBV6IYaQdiUIB8wIXJlLE02e4HmeAkpJDxsxOzKlVcTUC3IG85H5dYeTaZI+H0tD7u9oT2RsLDKaigl8ViUYmoxsEN8gIKNGojkFbMCQy2sVaCTVlYN1RFWeo+ilBqSRu5SIYe9gAXqNZRlcky7u9vymn2DsbcIrVEs/WoUyM07zGjFt0hZyUdKVbYbpgFp3tiaYNYm+Qc6j7TNYnAurq4FzugVLDj2z0Ha7hKJt1nIpiZtqYPLMc5fFRyp27KlLqjkJTx2vnCXsWGmY0HdB2PRxmQQLjhlI1/RW+FRD0h4lh9D9pn06w5raaBD9ofKaA4MZDtL/r1PAxkyjKQ48/w9T+m4k1qHlhSGg5LBO1/iDwrCynojksD7W+IPCJ1nMzI7c+Kvh+8UW3R008J9YpRYI9Nu79EnXgBbVoxQba3PHvnWN2A/l6R5xGcp2nCYiZ2+UaxhSA2R1WOl+crMP8yZtYxhKrhJuyKlWqU3DoxV0IZSDxm9wWKFSijjL2iKxHBW4zAOvz4TS/hvEn2G4dabsByiTTa4aL70P3z1jgP8yINHqb/uIUSCjboo3Ssu7IonfaoRYdFEN79GP/EOyqLr7YVKVGrkjCo/s1xDf3l/CIiUR8z2kwJt+7Uw9RCCHUU94dGmI3p7Ni+/qkyzsbYW5apVUGpkadPrKnee+HSP8wB+GcXjGR973mDVtykrC9ROR7IfquioXvdUBY9spGPqqJyfs7AO2Km9UCDSmLnxQfuD7yZ2LMWOrFmPOcAUnt7cshM5DRVECpceZnXoqRmAQcjcXElRQWJzt1V7LSS0RjIC4jZKEgofZkEErqpk26RrqMoSYZf4lfEBYGnIa0iAnTvtI8eB7Cp/Tb0nfaZgeQ7LxuOv7Cp/Tc/SL6tPprtFCn1F8Igfax6Y8ML0j0F8KwPtU+8HhnUsOf6ZTbvXTwt6xTu3esvJopSOCs2KnMnt05TpMauQ9coi056OmxXjGfP6xrNI79I8hHSFbJP/AGMeOjCYwpE0J7ExAVyp0bpDhnBziMVyjAj8pB1mZjeI1x8hLuCTee38ug7TBWz330U3uGz14TQ7MpXS9rPvbwPG0kl1sMnxIK0qNkGV93PmJm/xRX36wp7vQp0/aWvlvHj6TUU6htYix0v2zF7aqh8XUIXpo7UznvDdsBBG3LppUohj8JkDDsC4c7+/p0kBGku7WqgIFAsahz4XWUvwuE3am6LqrKGYiwdrRbVq79U/y0/dixhk/wCqNFfzZTsD95yo1ly6zndWPUZSNBdyx6q3VIAscq2AHDSdJAHfpOFxGM0yV9BdCZs+4ZnvMq1Lk6yYmy885EwjRQsmVKgz9IsS+9h6l9fZuDztHVR9DeQ1D/D1e5HP0g8i4mNFlGkegvhWCdq9dfCYTot0F8KwZtbrL4TKIQy23esnJvtFO7c1T9/2ijrBGa4mRs0aW74r/wC6SaRZs4Sew24G0YCd7ytHnPiMszxkG90x5iNQC1YicIjVeP8AWAJGwkFW1pYfSVqpjIVms/DB38MoBz3mp5/la822y7W8lU85gvwfWVaRvotdR3C83uDW28RqpDjvEVqkwXckggyZ24EXHcZgcXf29U7yj3tQHjvC89BVgwBHcZ55iiPa1BkxqVKoC8Qd4yfj0eeGg2DU3KNUlPZnf3gDlcWFpWY3N755k95lbBOVpuu/v3qXY8bgDKTBx99YZLpovg52NrcWyGWgnDoAMgMhykPt1LE81XLhOe27ifKb1B7Eloyo2VuJIEQqdxHbllGM13XzaNQo5zGXjmPznPLnMYrVdZA/wK3ge3ylisel9JXq29jV7Sj3+UWf+Ro6DKB6C+FYN2qemvhMIUD0F8K+kGbUPTXwmMhWZvbn/wAf7/tFOba0Tm/2ilFgj00xcCM3ydPSMVCZYSmqi5yiFaOkbq3OXGUWfpg8Lyaq7OcslGUidABGQrLiAnhYesfaVsNUNrX0y75Ox/zFHE+kqVZdYdGUakZCsOfhhwadZPzKVrDttPQ9h1t9BfNwAp/UJ5VsLFeyxa3NqdYGg+eWek9A2TVeg4z36RIUG+ajsiyxirUzTi6N+hyAf0tPP8Tb/kVMrIatUF9Amc9Fuji3/oM8+xqEYqouYPtmt+pbmTjpSRYwybqDM9K7m5zEfVay2GrZDtAiDX+3ACV2qXa/kM+EpRNsfn/piB75HcmPVT2QmHA3y8znOK3vCOxcpLuWHZxlXDNerU7AFAg+GLJBnRz5zl848AWmCVMRK7noVB203P0lqsMpS/LU7qVT0iy/yFaDKHUXwrBu1D018MIYc9BfCsG7T6y+ExkB6Z7bXVTxNFO7a6q+JhFHWCPTUBQOy8Y12nSxJ7o1mAERFpM4xVRIAC7d0c12MlsEW/l5xrEqyvkKlh/plxO37wcT0ge8GWFLnlBIMWXH0lKsJYQ2GZkGJyP1miGRWXJ1PYynlnPQcDWLKAcyLBu+efPp3jMc5sNmV96ilQahVSoOM0hUeh4CqtSkp/OLK3bvTFVkvjKzE33KtUDPK9zDexcWEaxPu6liOwNBWJ3Eeodd6rUccAxJk0ujt8Iq7G1hq2ueixiUj6RyKSbnU3Jk2+ijXOVxEtO06IEluolZ6+WVxrGbxPGL1hJa9SUcCSalTP8Altlwk9XT/byrs5vfML51FyzteGuAvoVVV4m8THsEYaZGjfWdVv8AbxRiOsMpRGlX+m/pL75g5W+8oNkKv9Jz9IJYMtBGG6i+FYP2memvIwhhz0F8KwbtQ9NfCYyFYC211V8Z9Jyd211F8X2nI6wR6aN2AyGuhjRTc66SdKajhc6yXd8uyTui/rZAlIDPz5SGsSxt+USw7cJA4AHfCv1iy/EVmW55ZyfDYlGbcIs2gNsmkTcYsLTzLWubkJloYZdQsXTL7CmMyO+UqrbzE8OHcJYcFtZC6gD1giqGk7KrjKaTYjMii+dOoFVv0N2zOtx85rtl4f8Ah0BzJRSctYZPgiXQlQcowF8rhkbgrSpiKhqVCb9EEt3M0czlUKnQZrUJ6qyPD2cXUgrpcHIxYr6GT+E43rWB+mZiWlf80clB/wCex5SwlMDXXjnrC2BRK4w5iOGPAy0xI6q7x+gkDriG/Nu+HozJs1JFbEkqtj1joL3JlTDIVqg36XbwEvNh1GbNvHsBuZUdm9olslVgTlqIywV6F0O8O/TnGvTPDnOIZIW78+UmU4Qte2ko1NKnfTcfSX6r3GsH1D1++nVH0mlhloHon3a+FfSDNpHpL4TCFA9BfCsG7T6w8MZAYG2x8NfGPQxTm1/hjxr6GKOhGahWMeWP+mKKSOgjtI37YooyEZVcE+ctUQFUCKKFmiOGfqZFW1tFFMjMq1NDyM3WAACKvFUpgjsyiiiT+Gj9JMThhURkPRDqRfslbA7PrIWLVBZrBEQWVQJ2KaOAel3piJQePrFFMY4xPA24Rtm4sT5xRRhRlQQfiX3FuM3uAO8xRRkBhSlusoYG1wGjna3HOcik1o7whdieEp4gdY/oqX+UUU0sBHQHRPQHhWDtpdYeGKKFBYH2r8IeKKKKOsEP/9k=" alt="Foto">
        </div>
        <div class="md:w-7/12">
          <p class="mb-3 md:mb-7 fadein-left fadeins-1">
            &nbsp; &nbsp; &nbsp;  I am a highly motivated senior in Computer Science at Southern New Hampshire University, bringing a year of substantial internship experience. Dedicated to Software Engineering and Development, I am passionate about employing creative problem-solving skills to overcome technological challenges. 
          </p>
          <p class="mb-3 fadein-left fadeins-2">
            &nbsp; &nbsp; &nbsp;My enthusiasm for technology is paralleled by my passion for fostering inclusivity and connection. In the New England Community and University, I've played a key role in launching several multicultural initiatives, fostering a diverse and cohesive academic environment. As I stand at the start of my professional career, I am driven to merge these dual passions: leveraging technology to create solutions that resonate across diverse user bases and building platforms that celebrate and encourage diversity in all its forms.
          </p>
        </div>

      </section>

    </article>
  </div>

  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center">
          <div class="h-[1px] w-10 bg-amber-200 md:w-20 aos-init aos-animate" data-aos="zoom-in-left"
            data-aos-duration="600"></div>
          &nbsp; Skills
        </div>
      </header>
      <section>
        <div>
          <ul class="flex flex-wrap text-sm font-medium text-center text-gray-500 dark:text-gray-400 mb-5">
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
                :class="{ 'text-amber-200 bg-amber-200 bg-opacity-10': activeTab === 1 }" @click="activeTab = 1">Tech Stack</button>
            </li>
            <li class="mr-2">
              <button class="inline-block px-4 py-3 rounded-lg hover:text-white"
                :class="{ 'text-amber-200 bg-amber-200 bg-opacity-10': activeTab === 2 }" @click="activeTab = 2">Tools</button>
            </li>
          </ul>
        </div>
        <div v-show="activeTab === 1">
          <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tech" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border border-amber-200 px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]  "
                    :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0 ">{{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div v-show="activeTab === 2">
          <div class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12">
            <div v-for="item in tools" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border border-amber-200 px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3">
                <div class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in">
                  <img alt="HTML" loading="lazy" width="32" height="32" decoding="async" data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]  "
                    :src="item.imageUrl" style="color: transparent;">
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div class="tech font-medium text-secondary transition-all duration-300 translate-y-0 ">{{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </article>
  </div>
</template>

<style>
.fadein-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadeins-1 {
  animation-delay: 500ms;
}

.fadeins-2 {
  animation-delay: 800ms;
}

.img-tech,
.tech {
  transition: transform 0.3s ease;
}

.item-tech:hover .img-tech {
  transform: scale(1.3);
}

.item-tech:hover .tech {
  transform: translateY(-12px);
}

.item-tech:hover .status-tech {
  opacity: 1;
}
</style>
