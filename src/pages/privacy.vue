<script>
export default {
  name: 'IncosplayPrivacyPolicy',
  data() {
    return {
      currentLang: 'en',
      languageOptions: [
        { value: 'en', label: 'English' },
        { value: 'ko', label: '한국어' },
      ],
    }
  },
}
</script>

<template>
  <div class="pp-container" :lang="currentLang">
    <div class="pp-language-switch" aria-label="Language selector">
      <span class="pp-language-label">{{ currentLang === 'en' ? 'Language' : '언어' }}</span>
      <div class="pp-language-options">
        <button
          v-for="option in languageOptions"
          :key="option.value"
          class="pp-language-button"
          :class="{ 'is-active': currentLang === option.value }"
          type="button"
          :aria-pressed="currentLang === option.value"
          @click="currentLang = option.value"
        >
          {{ option.label }}
        </button>
      </div>
    </div>
    <div v-if="currentLang === 'en'">
      <header class="pp-header">
        <h1>Nuomet Privacy Policy</h1>
        <p class="pp-updated">
          Date of the latest edition: August 19, 2026
        </p>
      </header>

      <p class="pp-intro">
        This policy describes what information we process to ensure that
        Incosplay, Timegram and other products and features offered by
        Nuomet Inc. ("Incosplay Products" or "Products"). For more
        tools and information, see the Incosplay Settings and Timegram
        Settings. The Privacy Policy defines the Incosplay User Information
        Protection Policy.
      </p>

      <!-- 1. What types of information do we collect? -->
      <section class="pp-section">
        <h2>1. What types of information do we collect?</h2>
        <p>
          We need to process information about you to provide Incosplay
          Products. Types of information we collect depend on how you use our
          Products. To learn how to access the information we collect, and how
          to delete it, go to Incosplay Settings and Timegram Settings.
        </p>

        <h3>1.1 Your actions, the actions of other people, and the information you and they provide</h3>

        <h4>The information and content you provide</h4>
        <p>
          We collect content, messages, and other information you provide when
          using our Products, including when you register an account, create
          or share content, send messages, or interact with other people. This
          can include information from or about the content you provide (such
          as metadata), such as the location where a photo was taken, or the
          date a file was created. Our systems automatically process content
          and messages provided by you and others to analyze their context and
          content for the purposes described below. Learn more about
          controlling who can see what you share.
        </p>

        <h4>Communities and communications</h4>
        <p>
          We collect information about people, hashtags, accounts and groups
          you are associated with, and about your interaction with them in our
          Products — in particular, the people you are with most often, or the
          groups you have joined. We also collect contact information if you
          download, synchronize, or import it from your device (e.g. address
          book, call log, or SMS), and use it, for example, to help you and
          other users find people you may also know, for the other purposes
          listed below.
        </p>

        <h4>Your use of the Products</h4>
        <p>
          We collect information about how you use our Products, such as the
          types of content you view or interact with; the features you use;
          the actions you take; the people or accounts you interact with; and
          the time, frequency, and duration of your activities. For example,
          we record data about when you start and last use our Products, and
          what posts, videos, and other content you view in our Products.
        </p>

        <h4>Information about transactions made in our Products</h4>
        <p>
          If you use our Products for purchases or other financial
          transactions (for example, when you make a purchase in a
          marketplace), we collect purchase or transaction information. This
          includes payment information, such as account and delivery
          information, and contact information.
        </p>

        <h4>Other people's actions and the information they provide about you</h4>
        <p>
          We also obtain and analyze the content, messages, and information
          that other people provide when they use our Products. This can
          include information about you — for example, when other people
          share photos with you or comment on such a photo, send you a
          message, or upload, synchronize, or import your contact information.
        </p>

        <h3>1.2 Information from devices</h3>
        <p>
          As described below, we collect information from the computers,
          phones, connected TVs, and other internet-connected devices
          integrated with our Products, as well as information about those
          devices, and we combine such data across the different devices you
          use. For example, we use information collected about how you use our
          Products on your phone for more effective personalization of content
          (including advertising) or features you see on another device, such
          as a laptop or tablet, or to determine whether you took action in
          response to an ad shown on your phone on another device. We receive
          the following information from these devices:
        </p>
        <ul>
          <li>
            <strong>Device attributes:</strong> information such as operating
            system, hardware and software, battery level, signal strength,
            available memory, browser type, application and file names and
            types, and plugins.
          </li>
          <li>
            <strong>Actions on device:</strong> information about actions on
            the device, including whether a window is in the foreground or
            background, and mouse pointer movements (this helps distinguish
            bots from people).
          </li>
          <li>
            <strong>Identifiers:</strong> unique IDs, device IDs, and other
            IDs, such as apps or accounts you use, and a shared device ID (or
            other identifiers unique to Incosplay Products associated with the
            same device or account).
          </li>
          <li>
            <strong>Data from device settings:</strong> information you allow
            us to receive by enabling device settings, such as access to your
            location (GPS), camera, or photos.
          </li>
          <li>
            <strong>Network and connections:</strong> information such as your
            mobile operator or provider, language, time zone, mobile number, IP
            address, connection speed, and in some cases, information about
            other devices located nearby or on your network, so that we can
            perform operations such as streaming video from your phone to your
            TV.
          </li>
          <li>
            <strong>Cookie data:</strong> data from cookies stored on your
            device, including cookie identifiers and settings.
          </li>
        </ul>

        <h3>1.3 Information from partners</h3>
        <p>
          Advertisers, app developers, and publishers can send us information
          when they use Incosplay tools, Incosplay Login, our APIs and SDKs, or
          Incosplay pixels. These partners provide information about your
          actions outside of our Products — including information about your
          device, sites you visit, purchases you make, advertising you view,
          and how you use their services — regardless of whether you have an
          Incosplay account or are logged in. For example, a game developer can
          use our API to let us know which games you play, and a company can
          tell us about purchases you made in its store. We also receive
          information about your activities and purchases, both online and
          offline, from third-party data providers who are entitled to provide
          us with your information. Partners receive your data when you visit
          or use their services, or through third parties they work with. We
          require that, before providing us with any data about you, each
          partner has obtained the legal rights necessary to collect, use, and
          transfer your data.
        </p>
      </section>

      <!-- 2. How do we use this information? -->
      <section class="pp-section">
        <h2>2. How do we use this information?</h2>
        <p>
          We use the information we have (based on your settings) for the
          purposes listed below, as well as to provide and support Incosplay
          Products and related services described in the
          Incosplay User Agreement. The following describes how we use it.
        </p>

        <h3>2.1 To provide, personalize, and improve our Products</h3>
        <p>
          We use the information we have to provide our Products, including
          personalization features and content (such as your Incosplay Feed
          and ads) and recommendations (e.g. groups or events that may
          interest you, or topics you may want to follow) in and out of our
          Products. To create a unique and relevant experience for you, we use
          your connections, preferences, interests, and actions, based on data
          we collect and receive from you and others (including any
          specially-protected data you choose to provide); information about
          how you use and interact with our Products; and the people, places,
          or things you are associated with and interested in, in and outside
          our Products. Learn more about how we use information to
          personalize your use of Incosplay and Timegram, including features,
          content, and recommendations; you can also learn more about how we
          select the ads you see.
        </p>

        <h4>Information from various Incosplay Products and devices</h4>
        <p>
          We combine information about your activities across various
          Incosplay Products and different devices to create a more
          personalized and consistent experience across all the Incosplay
          Products you use, wherever you use them. We may also use this to
          make using our Products more convenient, e.g. automatically filling
          in your registration information (such as a phone number) from one
          Incosplay Product when you sign in to another Product.
        </p>

        <h4>Location information</h4>
        <p>
          We use location information — for example, your current location,
          where you live, places you like to visit, and the businesses and
          people near you — to provide, personalize, and improve our Products,
          including the ads shown to you and other people. Location
          information can be derived from sources such as the precise location
          of your device (if you have allowed us to collect this information),
          IP addresses, and information collected during your and others' use
          of Incosplay Products (e.g. visits or events you attend).
        </p>

        <h4>Product research and development</h4>
        <p>
          We use the information available to us to develop, test, and improve
          our Products, including through surveys and research, and by
          testing and troubleshooting new products and features.
        </p>

        <h4>Advertising and other sponsored content</h4>
        <p>
          We use the information we have about you — including information
          about your interests, actions, and connections — to select and
          personalize the ads, offers, and other sponsored content we show
          you.
        </p>

        <h3>2.2 Provide measurement, analytics, and other business services</h3>
        <p>
          We use the information available to us (including your activity
          outside our Products, such as the sites you visit and ads you view)
          to help advertisers and other partners measure the performance and
          distribution of their advertising and services, and understand what
          types of people use their services and how people interact with
          their sites, apps, and services.
        </p>

        <h3>2.3 Ensure security, integrity, and protection</h3>
        <p>
          We use the information we have to verify accounts and activity,
          combat harmful conduct, identify and prevent spam and other harmful
          content, maintain the integrity of our Products, and improve
          security both within and outside the Incosplay Products. For
          example, we use available data to investigate suspicious activity or
          violations of our terms and conditions, and to identify situations
          where someone may need our help.
        </p>

        <h3>2.4 To communicate with you</h3>
        <p>
          We use the information available to us to send you marketing
          offers, communicate with you about our Products, and inform you of
          our policies and terms. We also need this information to respond to
          your inquiries.
        </p>

        <h3>2.5 Research and innovation for the public good</h3>
        <p>
          We use the information available to us (including information from
          collaborating research partners) to conduct and support research and
          innovation on topics of general social welfare, technological
          advancement, public interest, health, and well-being.
        </p>
      </section>

      <!-- 3. How is this information shared? -->
      <section class="pp-section">
        <h2>3. How is this information shared?</h2>
        <p>We share your information with others in the following ways:</p>

        <h3>3.1 The people and accounts you communicate and share with</h3>
        <p>
          When you communicate and share information using our Products, you
          choose the audience for what you share. For example, if you post on
          Incosplay, you choose the audience for that post: all Incosplay
          users, or subscribers only. Similarly, when you use Incosplay to
          communicate with people or companies, those people and companies can
          see the content you send. Your community can also see the actions
          you take in our Products, including interactions with advertising
          and sponsored content. We also let accounts see who viewed their
          stories on Incosplay or Timegram.
        </p>
        <p>
          Public information is visible to everyone, in and out of our
          Products, even to people without an account. This includes your
          Incosplay username; any information you share publicly; information
          in your public Incosplay profile; and content you share on an
          Incosplay Page, a public Incosplay account, or any other public
          venue. You, other Incosplay and Timegram users, and we can provide
          access to or send public information to anyone, in or outside our
          Products, including through other Incosplay Products, search
          results, or tools and APIs. Public information can also be viewed,
          reposted, downloaded, and accessed through third-party services such
          as search engines, APIs, and traditional media (e.g. TV), as well as
          through applications, sites, and other services integrated with our
          Products.
        </p>

        <h3>3.2 Content about you that other people share and re-share</h3>
        <p>
          You should be careful when choosing your audience, since people who
          can see your activity on our Products may share that information
          with others, in and outside our Products, including people and
          companies outside your chosen audience. For example, when you share
          a post or send a message to certain accounts, they may download,
          screenshot, or repost that content for others across various
          Incosplay Products. Likewise, when you comment on someone else's
          post or react to their content, your comment or reaction is visible
          to anyone who can see that person's content, and they may later
          change the audience for it. People can also use our Products to
          create content about you and share it with their own chosen
          audience — for example, sharing a photo with you in a story,
          mentioning or tagging you at a location in a post, or sharing
          information about you in their posts or messages. If you want
          information about you that others have shared on our Products
          removed, use our content complaint procedure.
        </p>

        <h3>3.3 Information about your active status or presence in our Products</h3>
        <p>
          Members of your communities can see signals indicating your active
          status on our Products, including on Timegram, or the last time you
          used our Products.
        </p>

        <h3>3.4 Apps, sites, and third-party integrations in or using our Products</h3>
        <p>
          When you choose to use third-party apps, sites, or other services
          that use, or are integrated with, our Products, they can receive
          information about what you post or share. For example, a game
          developer or site may receive information about your activity, or
          obtain a comment or link you shared on Incosplay. Likewise, when you
          download or use such third-party services, they may access your
          public Incosplay profile and any information you share with them.
          Apps and sites you use can get a list of your Incosplay subscribers
          if you grant them access; however, they cannot obtain any other
          information about your subscribers on Incosplay or Timegram
          (although your subscribers may, of course, choose to share that
          information themselves). Information shared with such third-party
          services is governed by their own terms and policies, not this
          policy. Devices and operating systems that provide native versions
          of Incosplay and Timegram (i.e. devices and OS for which we have not
          developed our own dedicated apps) will have access to all
          information you choose to share with them, including information
          that your subscribers share with you, so that they can provide you
          with basic functionality.
        </p>

        <h3>3.5 New owner</h3>
        <p>
          If our Products or their assets become wholly or partially owned or
          controlled by another entity, we may transfer your information to
          the new owner.
        </p>

        <h3>3.6 Sharing information with third-party partners</h3>
        <p>
          We work with third-party partners to help us deliver and improve our
          Products, or to use Incosplay tools to promote their business.
          Through this cooperation, our companies operate and provide free
          services to people around the world. We do not sell, and will never
          sell, your information to anyone. We also strictly limit how
          partners may use and disclose the data we provide. Below are the
          types of third parties we share information with:
        </p>
        <ul>
          <li>
            <strong>Partners who use our analytics services.</strong> We
            provide aggregated statistics that help people and businesses
            analyze user interactions with their posts, ads, Incosplay Pages,
            videos, and other content, in and outside the Incosplay Products.
            For example, owners of Incosplay and Timegram accounts receive
            information about the number of people or accounts who viewed,
            commented on, or reacted to their posts, along with aggregated
            demographic and other information to help them analyze
            interactions with their Incosplay Page or account.
          </li>
          <li>
            <strong>Advertisers.</strong> We provide advertisers with reports
            on the types of people who view their ads and on ad performance,
            but we do not share information that identifies you personally
            (such as your name or email address that could itself be used to
            contact or identify you) without your permission. For example,
            advertisers may receive aggregated demographic and interest
            information from us (e.g. an ad was viewed by a woman aged 25–34
            in Madrid who is interested in software development). We also
            provide them with evidence that a particular ad led you to make a
            purchase or take another action with the advertiser.
          </li>
          <li>
            <strong>Measurement partners.</strong> We share information about
            you with companies that aggregate it to provide our partners with
            analytics and measurement reports.
          </li>
          <li>
            <strong>Partners offering goods and services in our Products.</strong>
            When you subscribe to paid content or buy something from a seller
            within our Products, the content creator or seller may receive
            your public information and other information you share with
            them, as well as information needed to complete the transaction,
            including shipping and contact details.
          </li>
          <li>
            <strong>Vendors and service providers.</strong> We provide
            information and content to vendors and service providers who
            support our operations, such as maintaining technical
            infrastructure, analyzing how our Products are used, providing
            customer support, processing payments, and conducting surveys.
          </li>
          <li>
            <strong>Researchers and scientists.</strong> We also provide
            information and content to research partners and scientists to
            conduct research that advances science and innovation relevant to
            our business or mission, and that contributes to discoveries and
            developments in areas of general social welfare, technological
            advancement, public interest, health, and well-being.
          </li>
          <li>
            <strong>Law enforcement agencies and official inquiries.</strong>
            We provide information to law enforcement or other authorities
            upon formal request, in the situations described below.
          </li>
        </ul>
      </section>

      <!-- 4. How can you manage or delete information about yourself? -->
      <section class="pp-section">
        <h2>4. How can you manage or delete information about yourself?</h2>
        <p>
          We give you the ability to access, correct, transfer, and delete
          your data. For more information, see Incosplay Settings and Timegram
          Settings.
        </p>
        <p>
          We store data for as long as it is necessary to provide our
          Incosplay Services and Products, or until your account is deleted,
          whichever happens first. The retention period is determined on a
          case-by-case basis depending on factors such as the nature of the
          data, the purpose of its collection and processing, and relevant
          legal or operational reasons for retaining it. For example, when you
          search for something on Incosplay, you can access and delete that
          query from your search history at any time, but it will not be
          deleted from our search logs until 6 months later. If you send us a
          copy of a government-issued ID to verify your account, we delete
          that copy 30 days after review, unless otherwise indicated.
        </p>
        <p>
          When you delete your account at your request, we delete everything
          you have posted, such as your photos and status updates, and you
          will not be able to recover this information afterward. Information
          about you that others have shared is not part of your account and
          cannot be deleted by you. You can delete your account at any time in
          the Incosplay Settings and Timegram Settings.
        </p>
      </section>

      <!-- 5. How do we respond to legal requests or prevent harm? -->
      <section class="pp-section">
        <h2>5. How do we respond to official requests or prevent harm?</h2>
        <p>
          We access, preserve, and share your information with regulators, law
          enforcement authorities, and others:
        </p>
        <ul>
          <li>
            In response to a formal legal request (such as a search warrant,
            court order, or subpoena), if we have a good-faith belief that the
            law requires us to do so. Among other things, this may include
            responding to formal requests from countries other than the
            United States, where we have a good-faith belief that a response
            is required under the laws of that country, affects users in that
            country, and is consistent with internationally recognized
            standards.
          </li>
          <li>
            If we have a good-faith reason to believe it is necessary to:
            detect, prevent, or stop fraud, unauthorized use of the Products,
            violations of our terms, or other harmful or illegal acts; protect
            ourselves (including our rights, property, or Products), you, or
            others, including in connection with investigations or regulatory
            inquiries; or prevent death or imminent harm to health.
          </li>
        </ul>
        <p>
          For example, where necessary, we provide and receive information
          from third-party partners about the reliability of your account in
          order to prevent fraud, abuse, and other harmful activity in and
          outside our Products.
        </p>
        <p>
          We may retain information we have collected about you (including
          financial transaction data related to purchases made through our
          Products) and access it for a longer period if it is subject to a
          formal legal request or legal obligation, a government investigation,
          an investigation into possible violations of our terms or policies,
          or is otherwise necessary to prevent harm. We also retain information
          from accounts disabled for violating our User Agreement for at least
          a year, to prevent repeat violations or further violations of our
          terms.
        </p>
      </section>

      <!-- 6. Global data processing and transfer -->
      <section class="pp-section">
        <h2>6. How do we process and transfer data within our global services?</h2>
        <p>
          We share information globally, within Incosplay Companies, with our
          external partners, and with the people you communicate and share
          content with, in accordance with this policy. For example, your
          information may be transferred, stored, and processed in the United
          States or in other countries outside your country of residence, for
          the purposes described in this policy. Such data transfers are
          necessary to provide the services described in the
          <a
            href="http://safari-reader//incosplay.top/agreement"
            target="_blank"
            rel="noopener"
          >Incosplay User Agreement</a>, and to operate and deliver our Products to you worldwide. We rely
          on standard contractual clauses, European Commission adequacy
          decisions for the relevant countries, and your consent to transfer
          data to the United States and other countries.
        </p>
      </section>

      <!-- 7. Changes to this policy -->
      <section class="pp-section">
        <h2>7. How will we notify you of changes to this policy?</h2>
        <p>
          We will notify you in advance of changes to this policy and give you
          the opportunity to review the revised version before deciding
          whether to continue using our Products.
        </p>
      </section>

      <!-- 8. Contact -->
      <section class="pp-section">
        <h2>8. How do I ask a question?</h2>
        <p>
          If you have questions about this policy, you can contact us as
          described below.
        </p>
        <address class="pp-address">
          Contact
          email:
          <a href="mailto:support@incosplay.top?subject=Policy%20question">Nuomet098772@gmail.com</a>
        </address>
      </section>
    </div>
    <div v-else>
      <header class="pp-header">
        <h1>누오멧 개인정보 처리방침</h1>
        <p class="pp-updated">
          최신 개정일: 2026년 8월 19일
        </p>
      </header>

      <p class="pp-intro">
        본 정책은 누오멧 Inc.가 제공하는 Incosplay, Timegram 및 기타 제품과 기능("Incosplay 제품" 또는 "제품")이 제공되도록 하기 위해 당사가 어떤 정보를 처리하는지 설명합니다. 더 많은 도구와 정보는 Incosplay 설정 및 Timegram 설정을 참조하십시오. 본 개인정보 처리방침은 Incosplay 사용자 정보 보호 정책을 정의합니다.
      </p>

      <!-- 1. What types of information do we collect? -->
      <section class="pp-section">
        <h2>1. 어떤 유형의 정보를 수집하나요?</h2>
        <p>
          당사는 Incosplay 제품을 제공하기 위해 귀하에 관한 정보를 처리해야 합니다. 당사가 수집하는 정보의 유형은 귀하가 제품을 이용하는 방식에 따라 달라집니다. 당사가 수집하는 정보에 접근하는 방법과 해당 정보를 삭제하는 방법을 알아보려면 Incosplay 설정 및 Timegram 설정으로 이동하십시오.
        </p>

        <h3>1.1 귀하의 활동, 다른 사람의 활동, 그리고 귀하와 그들이 제공하는 정보</h3>

        <h4>귀하가 제공하는 정보와 콘텐츠</h4>
        <p>
          당사는 귀하가 제품을 이용할 때 제공하는 콘텐츠, 메시지 및 기타 정보를 수집합니다. 여기에는 계정을 등록하거나, 콘텐츠를 만들거나 공유하거나, 메시지를 보내거나, 다른 사람과 상호작용하는 경우가 포함됩니다. 여기에는 사진이 촬영된 위치나 파일이 생성된 날짜와 같은 메타데이터 등 귀하가 제공한 콘텐츠에서 비롯되거나 해당 콘텐츠에 관한 정보가 포함될 수 있습니다. 당사 시스템은 아래에 설명된 목적을 위해 귀하와 다른 사람이 제공한 콘텐츠와 메시지의 맥락과 내용을 분석하도록 자동으로 처리합니다. 귀하가 공유하는 내용을 누가 볼 수 있는지 제어하는 방법에 대해 자세히 알아보십시오.
        </p>

        <h4>커뮤니티와 커뮤니케이션</h4>
        <p>
          당사는 귀하가 관련되어 있는 사람, 해시태그, 계정 및 그룹에 관한 정보와 제품 내에서 귀하가 그들과 상호작용하는 방식에 관한 정보를 수집합니다. 특히 귀하가 가장 자주 함께하는 사람이나 가입한 그룹에 관한 정보를 수집합니다. 또한 귀하가 기기에서 연락처 정보를 다운로드, 동기화 또는 가져오는 경우(예: 주소록, 통화 기록 또는 SMS) 해당 정보를 수집하며, 예를 들어 귀하와 다른 사용자가 서로 알 수도 있는 사람을 찾도록 돕고 아래에 나열된 기타 목적을 위해 이를 사용합니다.
        </p>

        <h4>귀하의 제품 이용</h4>
        <p>
          당사는 귀하가 제품을 어떻게 이용하는지에 관한 정보를 수집합니다. 예를 들어 귀하가 보거나 상호작용하는 콘텐츠 유형, 사용하는 기능, 수행하는 활동, 상호작용하는 사람 또는 계정, 그리고 활동의 시간, 빈도 및 기간 등이 포함됩니다. 예를 들어 당사는 귀하가 제품 이용을 시작한 시점과 마지막으로 이용한 시점, 그리고 제품 내에서 본 게시물, 동영상 및 기타 콘텐츠에 관한 데이터를 기록합니다.
        </p>

        <h4>제품 내 거래 정보</h4>
        <p>
          귀하가 구매 또는 기타 금융 거래를 위해 제품을 이용하는 경우(예: 마켓플레이스에서 구매하는 경우), 당사는 구매 또는 거래 정보를 수집합니다. 여기에는 계정 및 배송 정보, 연락처 정보와 같은 결제 정보가 포함됩니다.
        </p>

        <h4>다른 사람의 활동 및 그들이 귀하에 대해 제공하는 정보</h4>
        <p>
          당사는 다른 사람이 제품을 이용할 때 제공하는 콘텐츠, 메시지 및 정보를 또한 취득하고 분석합니다. 여기에는 귀하에 관한 정보가 포함될 수 있습니다. 예를 들어 다른 사람이 귀하와 사진을 공유하거나 해당 사진에 댓글을 남기거나, 귀하에게 메시지를 보내거나, 귀하의 연락처 정보를 업로드, 동기화 또는 가져오는 경우가 이에 해당합니다.
        </p>

        <h3>1.2 기기에서 수집하는 정보</h3>
        <p>
          아래에 설명된 바와 같이, 당사는 제품과 통합된 컴퓨터, 휴대전화, 연결된 TV 및 기타 인터넷 연결 기기에서 정보와 해당 기기에 관한 정보를 수집하며, 귀하가 사용하는 여러 기기 전반에서 이러한 데이터를 결합합니다. 예를 들어 당사는 귀하가 휴대전화에서 제품을 어떻게 이용하는지에 관해 수집한 정보를 사용하여 노트북이나 태블릿과 같은 다른 기기에서 보게 되는 콘텐츠(광고 포함)나 기능을 더 효과적으로 개인화하거나, 귀하가 휴대전화에 표시된 광고에 대한 반응으로 다른 기기에서 활동을 했는지 판단할 수 있습니다. 당사는 이러한 기기에서 다음 정보를 받습니다.
        </p>
        <ul>
          <li>
            <strong>기기 속성:</strong> 운영 체제, 하드웨어 및 소프트웨어, 배터리 수준, 신호 강도, 사용 가능한 메모리, 브라우저 유형, 애플리케이션 및 파일 이름과 유형, 플러그인 등의 정보.
          </li>
          <li>
            <strong>기기 내 활동:</strong> 창이 전면 또는 백그라운드에 있는지 여부, 마우스 포인터 움직임 등 기기에서의 활동에 관한 정보(이는 봇과 사람을 구분하는 데 도움이 됩니다).
          </li>
          <li>
            <strong>식별자:</strong> 고유 ID, 기기 ID 및 귀하가 사용하는 앱이나 계정과 같은 기타 ID, 그리고 동일한 기기 또는 계정과 관련된 Incosplay 제품에 고유한 공유 기기 ID(또는 기타 식별자).
          </li>
          <li>
            <strong>기기 설정 데이터:</strong> 위치(GPS), 카메라 또는 사진 접근 권한과 같이 귀하가 기기 설정을 활성화하여 당사가 받을 수 있도록 허용한 정보.
          </li>
          <li>
            <strong>네트워크 및 연결:</strong> 이동통신사 또는 제공업체, 언어, 시간대, 휴대전화 번호, IP 주소, 연결 속도, 그리고 경우에 따라 귀하의 기기 근처 또는 네트워크에 있는 다른 기기에 관한 정보. 이는 예를 들어 휴대전화에서 TV로 비디오를 스트리밍하는 등의 작업을 수행하기 위한 것입니다.
          </li>
          <li>
            <strong>쿠키 데이터:</strong> 쿠키 식별자 및 설정을 포함하여 귀하의 기기에 저장된 쿠키의 데이터.
          </li>
        </ul>

        <h3>1.3 파트너로부터 받는 정보</h3>
        <p>
          광고주, 앱 개발자 및 게시자는 Incosplay 도구, Incosplay 로그인, 당사의 API 및 SDK 또는 Incosplay 픽셀을 사용할 때 당사에 정보를 보낼 수 있습니다. 이러한 파트너는 귀하가 Incosplay 계정을 보유하고 있거나 로그인했는지 여부와 관계없이, 귀하의 기기, 방문한 사이트, 구매 내역, 본 광고 및 해당 서비스 이용 방식 등 제품 외부에서의 귀하의 활동에 관한 정보를 제공합니다. 예를 들어 게임 개발자는 당사의 API를 사용하여 귀하가 어떤 게임을 하는지 알려줄 수 있고, 회사는 귀하가 해당 매장에서 구매한 내역을 당사에 알려줄 수 있습니다. 또한 당사는 귀하의 정보를 제공할 권리가 있는 제3자 데이터 제공업체로부터 온라인 및 오프라인에서의 귀하의 활동과 구매에 관한 정보를 받습니다. 파트너는 귀하가 그들의 서비스를 방문하거나 이용할 때, 또는 그들이 협력하는 제3자를 통해 귀하의 데이터를 받습니다. 당사는 각 파트너가 귀하에 관한 데이터를 당사에 제공하기 전에 해당 데이터를 수집, 사용 및 이전하는 데 필요한 법적 권리를 확보하도록 요구합니다.
        </p>
      </section>

      <!-- 2. How do we use this information? -->
      <section class="pp-section">
        <h2>2. 이 정보를 어떻게 사용하나요?</h2>
        <p>
          당사는 귀하의 설정을 기반으로 보유한 정보를 아래에 나열된 목적뿐 아니라 Incosplay 사용자 계약에 설명된 Incosplay 제품 및 관련 서비스를 제공하고 지원하기 위해 사용합니다. 다음은 당사가 이를 어떻게 사용하는지 설명합니다.
        </p>

        <h3>2.1 제품 제공, 개인화 및 개선</h3>
        <p>
          당사는 보유한 정보를 사용하여 개인화 기능과 콘텐츠(예: Incosplay 피드 및 광고), 그리고 제품 안팎에서 귀하가 관심을 가질 수 있는 그룹이나 이벤트 또는 팔로우하고 싶을 수 있는 주제 등의 추천을 포함하여 제품을 제공합니다. 귀하에게 고유하고 관련성 높은 경험을 제공하기 위해, 당사는 귀하와 다른 사람으로부터 수집하고 받는 데이터를 기반으로 귀하의 연결, 선호, 관심사 및 활동(귀하가 제공하기로 선택한 특별 보호 데이터 포함), 귀하가 제품을 어떻게 이용하고 상호작용하는지에 관한 정보, 그리고 제품 안팎에서 귀하와 관련되어 있거나 귀하가 관심을 가진 사람, 장소 또는 사물을 사용합니다. 기능, 콘텐츠 및 추천을 포함하여 Incosplay 및 Timegram 이용을 개인화하기 위해 당사가 정보를 어떻게 사용하는지 자세히 알아볼 수 있으며, 귀하에게 표시되는 광고를 어떻게 선택하는지도 자세히 알아볼 수 있습니다.
        </p>

        <h4>다양한 Incosplay 제품 및 기기에서 얻는 정보</h4>
        <p>
          당사는 귀하가 사용하는 모든 Incosplay 제품 전반에서, 어디에서 이용하든 더 개인화되고 일관된 경험을 만들기 위해 다양한 Incosplay 제품과 서로 다른 기기에서의 귀하의 활동 정보를 결합합니다. 또한 예를 들어 귀하가 한 Incosplay 제품에 로그인할 때 다른 Incosplay 제품의 등록 정보(예: 전화번호)를 자동으로 채워 넣는 등 제품 이용을 더 편리하게 만들기 위해 이를 사용할 수도 있습니다.
        </p>

        <h4>위치 정보</h4>
        <p>
          당사는 현재 위치, 거주지, 방문하기 좋아하는 장소, 귀하 주변의 사업체와 사람 등 위치 정보를 사용하여 귀하와 다른 사람에게 표시되는 광고를 포함한 제품을 제공, 개인화 및 개선합니다. 위치 정보는 귀하가 당사에 이 정보를 수집하도록 허용한 경우 기기의 정확한 위치, IP 주소, 그리고 귀하와 다른 사람의 Incosplay 제품 이용 중 수집된 정보(예: 방문 또는 참석한 이벤트)와 같은 출처에서 파생될 수 있습니다.
        </p>

        <h4>제품 연구 및 개발</h4>
        <p>
          당사는 설문조사와 연구, 새로운 제품과 기능의 테스트 및 문제 해결을 포함하여 제품을 개발, 테스트 및 개선하기 위해 당사가 이용할 수 있는 정보를 사용합니다.
        </p>

        <h4>광고 및 기타 스폰서 콘텐츠</h4>
        <p>
          당사는 귀하의 관심사, 활동 및 연결에 관한 정보를 포함하여 귀하에 대해 보유한 정보를 사용하여 귀하에게 표시되는 광고, 제안 및 기타 스폰서 콘텐츠를 선택하고 개인화합니다.
        </p>

        <h3>2.2 측정, 분석 및 기타 비즈니스 서비스 제공</h3>
        <p>
          당사는 제품 외부에서의 귀하의 활동(예: 방문한 사이트 및 본 광고)을 포함하여 당사가 이용할 수 있는 정보를 사용하여 광고주와 기타 파트너가 광고 및 서비스의 성과와 배포를 측정하고, 어떤 유형의 사람들이 그들의 서비스를 이용하며 사람들이 그들의 사이트, 앱 및 서비스와 어떻게 상호작용하는지 이해하도록 돕습니다.
        </p>

        <h3>2.3 보안, 무결성 및 보호 보장</h3>
        <p>
          당사는 계정과 활동을 확인하고, 유해 행위를 방지하며, 스팸 및 기타 유해 콘텐츠를 식별하고 예방하고, 제품의 무결성을 유지하며, Incosplay 제품 내부와 외부 모두에서 보안을 개선하기 위해 보유한 정보를 사용합니다. 예를 들어 당사는 의심스러운 활동이나 약관 위반을 조사하고 누군가 도움이 필요할 수 있는 상황을 식별하기 위해 이용 가능한 데이터를 사용합니다.
        </p>

        <h3>2.4 귀하와의 커뮤니케이션</h3>
        <p>
          당사는 마케팅 제안을 보내고, 제품에 대해 귀하와 소통하며, 당사의 정책과 약관을 알려주기 위해 이용 가능한 정보를 사용합니다. 또한 귀하의 문의에 응답하기 위해서도 이 정보가 필요합니다.
        </p>

        <h3>2.5 공익을 위한 연구와 혁신</h3>
        <p>
          당사는 협력 연구 파트너로부터 받은 정보를 포함하여 이용 가능한 정보를 사용하여 일반적인 사회 복지, 기술 발전, 공익, 건강 및 웰빙에 관한 주제의 연구와 혁신을 수행하고 지원합니다.
        </p>
      </section>

      <!-- 3. How is this information shared? -->
      <section class="pp-section">
        <h2>3. 이 정보는 어떻게 공유되나요?</h2>
        <p>당사는 다음과 같은 방식으로 귀하의 정보를 다른 사람과 공유합니다.</p>

        <h3>3.1 귀하가 소통하고 공유하는 사람과 계정</h3>
        <p>
          귀하가 제품을 사용하여 정보를 소통하고 공유할 때, 귀하는 공유 대상자를 선택합니다. 예를 들어 Incosplay에 게시물을 올리는 경우 해당 게시물의 대상자를 모든 Incosplay 사용자로 할지, 구독자만으로 할지 선택합니다. 마찬가지로 귀하가 Incosplay를 사용하여 사람이나 회사와 소통할 때 해당 사람과 회사는 귀하가 보내는 콘텐츠를 볼 수 있습니다. 귀하의 커뮤니티는 또한 광고 및 스폰서 콘텐츠와의 상호작용을 포함하여 제품에서 귀하가 수행하는 활동을 볼 수 있습니다. 또한 당사는 계정이 Incosplay 또는 Timegram에서 자신의 스토리를 본 사람을 확인할 수 있도록 합니다.
        </p>
        <p>
          공개 정보는 계정이 없는 사람을 포함하여 제품 안팎의 모든 사람에게 표시됩니다. 여기에는 귀하의 Incosplay 사용자 이름, 귀하가 공개적으로 공유한 모든 정보, 귀하의 공개 Incosplay 프로필에 있는 정보, 그리고 Incosplay 페이지, 공개 Incosplay 계정 또는 기타 공개 장소에 공유한 콘텐츠가 포함됩니다. 귀하, 다른 Incosplay 및 Timegram 사용자, 그리고 당사는 다른 Incosplay 제품, 검색 결과, 도구 및 API를 포함하여 제품 안팎의 누구에게나 공개 정보에 대한 접근을 제공하거나 이를 보낼 수 있습니다. 공개 정보는 검색 엔진, API, TV와 같은 전통 미디어, 그리고 제품과 통합된 애플리케이션, 사이트 및 기타 서비스 등 제3자 서비스를 통해서도 조회, 재게시, 다운로드 및 접근될 수 있습니다.
        </p>

        <h3>3.2 다른 사람이 공유하고 재공유하는 귀하에 관한 콘텐츠</h3>
        <p>
          귀하는 대상자를 선택할 때 주의해야 합니다. 제품에서 귀하의 활동을 볼 수 있는 사람은 귀하가 선택한 대상자 밖의 사람과 회사를 포함하여 제품 안팎의 다른 사람과 해당 정보를 공유할 수 있기 때문입니다. 예를 들어 귀하가 특정 계정과 게시물을 공유하거나 메시지를 보내면, 그들은 다양한 Incosplay 제품 전반에서 다른 사람을 위해 해당 콘텐츠를 다운로드, 스크린샷 촬영 또는 재게시할 수 있습니다. 마찬가지로 귀하가 다른 사람의 게시물에 댓글을 달거나 콘텐츠에 반응하면, 귀하의 댓글 또는 반응은 그 사람의 콘텐츠를 볼 수 있는 누구에게나 표시되며, 그 사람은 나중에 해당 콘텐츠의 대상자를 변경할 수도 있습니다. 또한 사람들은 제품을 사용하여 귀하에 관한 콘텐츠를 만들고 자신이 선택한 대상자와 공유할 수 있습니다. 예를 들어 스토리에서 귀하와 사진을 공유하거나, 게시물에서 위치와 함께 귀하를 언급하거나 태그하거나, 게시물 또는 메시지에서 귀하에 관한 정보를 공유할 수 있습니다. 제품에서 다른 사람이 공유한 귀하에 관한 정보를 삭제하고 싶다면 당사의 콘텐츠 불만 제기 절차를 이용하십시오.
        </p>

        <h3>3.3 제품 내 활성 상태 또는 존재 정보</h3>
        <p>
          귀하의 커뮤니티 구성원은 Timegram을 포함한 제품에서 귀하의 활성 상태 또는 마지막으로 제품을 사용한 시간을 나타내는 신호를 볼 수 있습니다.
        </p>

        <h3>3.4 제품 내 또는 제품을 사용하는 앱, 사이트 및 제3자 연동</h3>
        <p>
          귀하가 제품을 사용하거나 제품과 통합된 제3자 앱, 사이트 또는 기타 서비스를 이용하기로 선택하면, 해당 서비스는 귀하가 게시하거나 공유한 내용에 관한 정보를 받을 수 있습니다. 예를 들어 게임 개발자나 사이트는 귀하의 활동에 관한 정보를 받거나 귀하가 Incosplay에서 공유한 댓글 또는 링크를 얻을 수 있습니다. 마찬가지로 귀하가 이러한 제3자 서비스를 다운로드하거나 이용할 때, 해당 서비스는 귀하의 공개 Incosplay 프로필과 귀하가 그들과 공유한 모든 정보에 접근할 수 있습니다. 귀하가 접근 권한을 부여하면 귀하가 사용하는 앱과 사이트는 귀하의 Incosplay 구독자 목록을 얻을 수 있습니다. 그러나 Incosplay 또는 Timegram의 귀하의 구독자에 관한 그 밖의 정보는 얻을 수 없습니다(물론 귀하의 구독자가 직접 해당 정보를 공유하기로 선택할 수는 있습니다). 이러한 제3자 서비스와 공유되는 정보는 본 정책이 아니라 해당 서비스의 약관과 정책의 적용을 받습니다. Incosplay 및 Timegram의 네이티브 버전을 제공하는 기기와 운영 체제(즉, 당사가 자체 전용 앱을 개발하지 않은 기기 및 OS)는 기본 기능을 제공하기 위해 귀하가 그들과 공유하기로 선택한 모든 정보에 접근할 수 있으며, 여기에는 귀하의 구독자가 귀하와 공유한 정보도 포함됩니다.
        </p>

        <h3>3.5 새로운 소유자</h3>
        <p>
          당사의 제품 또는 그 자산이 전부 또는 일부 다른 주체의 소유 또는 통제를 받게 되는 경우, 당사는 귀하의 정보를 새로운 소유자에게 이전할 수 있습니다.
        </p>

        <h3>3.6 제3자 파트너와의 정보 공유</h3>
        <p>
          당사는 제품을 제공하고 개선하는 데 도움을 받거나 Incosplay 도구를 사용하여 파트너의 사업을 홍보하기 위해 제3자 파트너와 협력합니다. 이러한 협력을 통해 당사의 회사들은 전 세계 사람들에게 무료 서비스를 운영하고 제공합니다. 당사는 귀하의 정보를 누구에게도 판매하지 않으며 앞으로도 절대 판매하지 않습니다. 또한 당사는 제공하는 데이터를 파트너가 사용하고 공개하는 방식을 엄격히 제한합니다. 아래는 당사가 정보를 공유하는 제3자의 유형입니다.
        </p>
        <ul>
          <li>
            <strong>당사의 분석 서비스를 사용하는 파트너.</strong> 당사는 사람들이 Incosplay 제품 안팎에서 게시물, 광고, Incosplay 페이지, 동영상 및 기타 콘텐츠와의 사용자 상호작용을 분석하는 데 도움이 되는 집계 통계를 제공합니다. 예를 들어 Incosplay 및 Timegram 계정 소유자는 자신의 게시물을 조회, 댓글 작성 또는 반응한 사람이나 계정 수에 관한 정보와, Incosplay 페이지 또는 계정과의 상호작용을 분석하는 데 도움이 되는 집계 인구통계 및 기타 정보를 받습니다.
          </li>
          <li>
            <strong>광고주.</strong> 당사는 광고를 보는 사람의 유형과 광고 성과에 관한 보고서를 광고주에게 제공하지만, 귀하의 허락 없이 귀하를 개인적으로 식별하는 정보(예: 그 자체로 귀하에게 연락하거나 귀하를 식별하는 데 사용될 수 있는 이름 또는 이메일 주소)는 공유하지 않습니다. 예를 들어 광고주는 당사로부터 집계된 인구통계 및 관심사 정보를 받을 수 있습니다(예: 마드리드에 거주하고 소프트웨어 개발에 관심이 있는 25~34세 여성이 광고를 봄). 또한 당사는 특정 광고가 귀하로 하여금 광고주와 구매 또는 기타 행동을 하도록 이끌었다는 증거를 제공합니다.
          </li>
          <li>
            <strong>측정 파트너.</strong> 당사는 파트너에게 분석 및 측정 보고서를 제공하기 위해 정보를 집계하는 회사들과 귀하에 관한 정보를 공유합니다.
          </li>
          <li>
            <strong>제품에서 상품과 서비스를 제공하는 파트너.</strong> 귀하가 제품 내에서 유료 콘텐츠를 구독하거나 판매자로부터 무언가를 구매하는 경우, 콘텐츠 제작자 또는 판매자는 거래를 완료하는 데 필요한 배송 및 연락처 세부 정보를 포함하여 귀하의 공개 정보와 귀하가 그들과 공유하는 기타 정보를 받을 수 있습니다.
          </li>
          <li>
            <strong>공급업체 및 서비스 제공업체.</strong> 당사는 기술 인프라 유지, 제품 이용 방식 분석, 고객 지원 제공, 결제 처리 및 설문조사 수행 등 당사의 운영을 지원하는 공급업체와 서비스 제공업체에 정보와 콘텐츠를 제공합니다.
          </li>
          <li>
            <strong>연구자 및 과학자.</strong> 또한 당사는 당사의 사업 또는 사명과 관련된 과학 및 혁신을 발전시키고, 일반적인 사회 복지, 기술 발전, 공익, 건강 및 웰빙 분야의 발견과 발전에 기여하는 연구를 수행하기 위해 연구 파트너와 과학자에게 정보와 콘텐츠를 제공합니다.
          </li>
          <li>
            <strong>법 집행 기관 및 공식 조회.</strong> 당사는 아래에 설명된 상황에서 공식 요청에 따라 법 집행 기관 또는 기타 당국에 정보를 제공합니다.
          </li>
        </ul>
      </section>

      <!-- 4. How can you manage or delete information about yourself? -->
      <section class="pp-section">
        <h2>4. 본인에 관한 정보를 어떻게 관리하거나 삭제할 수 있나요?</h2>
        <p>
          당사는 귀하가 데이터를 열람, 수정, 이전 및 삭제할 수 있는 기능을 제공합니다. 자세한 내용은 Incosplay 설정 및 Timegram 설정을 참조하십시오.
        </p>
        <p>
          당사는 Incosplay 서비스와 제품을 제공하는 데 필요한 기간 또는 귀하의 계정이 삭제될 때까지 중 먼저 도래하는 시점까지 데이터를 보관합니다. 보관 기간은 데이터의 성격, 수집 및 처리 목적, 그리고 해당 데이터를 보관해야 하는 관련 법적 또는 운영상 이유 등의 요소에 따라 사례별로 결정됩니다. 예를 들어 귀하가 Incosplay에서 무언가를 검색하면 언제든지 검색 기록에서 해당 쿼리에 접근하고 삭제할 수 있지만, 당사의 검색 로그에서는 6개월 후까지 삭제되지 않습니다. 귀하가 계정 확인을 위해 정부 발급 신분증 사본을 당사에 보내는 경우, 달리 명시되지 않는 한 당사는 검토 후 30일이 지나면 해당 사본을 삭제합니다.
        </p>
        <p>
          귀하의 요청에 따라 계정을 삭제하면, 당사는 귀하의 사진과 상태 업데이트 등 귀하가 게시한 모든 것을 삭제하며, 이후 귀하는 이 정보를 복구할 수 없습니다. 다른 사람이 귀하에 관해 공유한 정보는 귀하의 계정 일부가 아니므로 귀하가 삭제할 수 없습니다. 귀하는 Incosplay 설정 및 Timegram 설정에서 언제든지 계정을 삭제할 수 있습니다.
        </p>
      </section>

      <!-- 5. How do we respond to legal requests or prevent harm? -->
      <section class="pp-section">
        <h2>5. 공식 요청에 어떻게 대응하거나 피해를 방지하나요?</h2>
        <p>
          당사는 다음과 같은 경우 규제 기관, 법 집행 기관 및 기타 당사자와 귀하의 정보를 접근, 보존 및 공유합니다.
        </p>
        <ul>
          <li>
            수색영장, 법원 명령 또는 소환장과 같은 공식 법적 요청에 대응하기 위해, 법률상 그렇게 해야 한다는 선의의 믿음이 있는 경우. 특히 여기에는 미국 이외 국가의 공식 요청에 대응하는 경우가 포함될 수 있으며, 이때 당사는 해당 국가의 법률상 대응이 요구되고, 해당 국가의 사용자에게 영향을 미치며, 국제적으로 인정된 기준에 부합한다는 선의의 믿음을 가집니다.
          </li>
          <li>
            사기, 제품의 무단 사용, 당사 약관 위반 또는 기타 유해하거나 불법적인 행위를 탐지, 예방 또는 중지하기 위해, 당사(당사의 권리, 재산 또는 제품 포함), 귀하 또는 다른 사람을 보호하기 위해(조사 또는 규제 조회와 관련된 경우 포함), 또는 사망이나 건강에 대한 임박한 피해를 방지하기 위해 필요하다고 믿을 선의의 이유가 있는 경우.
          </li>
        </ul>
        <p>
          예를 들어 필요한 경우, 당사는 제품 안팎에서 사기, 남용 및 기타 유해 활동을 방지하기 위해 귀하의 계정 신뢰성에 관한 정보를 제3자 파트너와 제공하고 받습니다.
        </p>
        <p>
          당사는 제품을 통해 이루어진 구매와 관련된 금융 거래 데이터를 포함하여 귀하에 대해 수집한 정보를, 공식 법적 요청 또는 법적 의무, 정부 조사, 당사 약관 또는 정책 위반 가능성에 대한 조사 대상이거나, 그 밖에 피해를 방지하기 위해 필요한 경우 더 긴 기간 동안 보관하고 접근할 수 있습니다. 또한 당사는 반복 위반 또는 추가 약관 위반을 방지하기 위해 사용자 계약을 위반하여 비활성화된 계정의 정보를 최소 1년 동안 보관합니다.
        </p>
      </section>

      <!-- 6. Global data processing and transfer -->
      <section class="pp-section">
        <h2>6. 글로벌 서비스 내에서 데이터를 어떻게 처리하고 이전하나요?</h2>
        <p>
          당사는 본 정책에 따라 Incosplay 회사 내부, 외부 파트너, 그리고 귀하가 소통하고 콘텐츠를 공유하는 사람들과 전 세계적으로 정보를 공유합니다. 예를 들어 귀하의 정보는 본 정책에 설명된 목적을 위해 귀하의 거주 국가 밖의 미국 또는 기타 국가로 이전, 저장 및 처리될 수 있습니다. 이러한 데이터 이전은
          <a
            href="http://safari-reader//incosplay.top/agreement"
            target="_blank"
            rel="noopener"
          >Incosplay 사용자 계약</a>에 설명된 서비스를 제공하고, 전 세계에서 제품을 운영하고 제공하기 위해 필요합니다. 당사는 관련 국가에 대한 표준 계약 조항, 유럽위원회의 적정성 결정 및 미국과 기타 국가로 데이터를 이전하는 것에 대한 귀하의 동의에 의존합니다.
        </p>
      </section>

      <!-- 7. Changes to this policy -->
      <section class="pp-section">
        <h2>7. 본 정책의 변경 사항을 어떻게 통지하나요?</h2>
        <p>
          당사는 본 정책의 변경 사항을 사전에 통지하고, 귀하가 제품을 계속 사용할지 결정하기 전에 개정된 버전을 검토할 기회를 제공합니다.
        </p>
      </section>

      <!-- 8. Contact -->
      <section class="pp-section">
        <h2>8. 질문은 어떻게 하나요?</h2>
        <p>
          본 정책에 대해 궁금한 사항이 있는 경우 아래에 설명된 방법으로 당사에 문의할 수 있습니다.
        </p>
        <address class="pp-address">
          연락
          이메일:
          <a href="mailto:support@incosplay.top?subject=Policy%20question">Nuomet098772@gmail.com</a>
        </address>
      </section>
    </div>
  </div>
</template>

<style scoped>
.pp-container {
  max-width: 860px;
  margin: 0 auto;
  padding: 2.5rem 1.5rem 4rem;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
    'Helvetica Neue', Arial, sans-serif;
  color: #2b2d33;
  line-height: 1.7;
  font-size: 16px;
}

.pp-language-switch {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 0.75rem;
  margin-bottom: 1.25rem;
}

.pp-language-label {
  color: #6b6f76;
  font-size: 0.9rem;
}

.pp-language-options {
  display: inline-flex;
  padding: 0.2rem;
  border: 1px solid #d7dbe3;
  border-radius: 999px;
  background: #f6f7fa;
}

.pp-language-button {
  min-width: 76px;
  border: 0;
  border-radius: 999px;
  padding: 0.4rem 0.75rem;
  background: transparent;
  color: #555b66;
  cursor: pointer;
  font: inherit;
  font-size: 0.9rem;
  line-height: 1.2;
}

.pp-language-button.is-active {
  background: #2e9e6b;
  color: #fff;
  font-weight: 600;
}

.pp-header {
  border-bottom: 2px solid #e2e4ea;
  padding-bottom: 1rem;
  margin-bottom: 1.5rem;
}

.pp-header h1 {
  font-size: 1.9rem;
  font-weight: 700;
  margin: 0 0 0.4rem;
  color: #1a1c20;
}

.pp-updated {
  font-size: 0.9rem;
  color: #6b6f76;
  margin: 0;
}

.pp-intro {
  background: #f6f7fa;
  border-left: 4px solid #2e9e6b;
  padding: 1rem 1.25rem;
  border-radius: 6px;
  margin-bottom: 2rem;
  font-size: 0.97rem;
}

.pp-section {
  margin-bottom: 2.25rem;
}

.pp-section h2 {
  font-size: 1.3rem;
  font-weight: 700;
  color: #1a1c20;
  border-bottom: 1px solid #e2e4ea;
  padding-bottom: 0.5rem;
  margin-bottom: 1rem;
}

.pp-section h3 {
  font-size: 1.05rem;
  font-weight: 600;
  color: #33363d;
  margin: 1.25rem 0 0.5rem;
}

.pp-section h4 {
  font-size: 0.98rem;
  font-weight: 600;
  color: #2e9e6b;
  margin: 1rem 0 0.4rem;
}

.pp-section p {
  margin: 0 0 0.9rem;
  text-align: justify;
}

.pp-section ul,
.pp-section ol {
  margin: 0 0 1rem;
  padding-left: 1.5rem;
}

.pp-section li {
  margin-bottom: 0.6rem;
}

.pp-section a {
  color: #2e9e6b;
  text-decoration: none;
  word-break: break-word;
}

.pp-section a:hover {
  text-decoration: underline;
}

.pp-address {
  font-style: normal;
  background: #f6f7fa;
  border-radius: 6px;
  padding: 0.75rem 1rem;
  margin: 0;
}

@media (max-width: 600px) {

  .pp-language-switch {
    align-items: flex-start;
    flex-direction: column;
    gap: 0.45rem;
  }

  .pp-language-options {
    width: 100%;
  }

  .pp-language-button {
    flex: 1;
    min-width: 0;
  }

  .pp-container {
    padding: 1.5rem 1rem 3rem;
    font-size: 15px;
  }
}
</style>
