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
        <h1>Nuomet 개인정보 처리방침</h1>
        <p class="pp-updated">
          최신 개정일: 2026년 8월 19일
        </p>
      </header>

      <p class="pp-intro">
        본 정책은 Nuomet Inc.가 제공하는 Incosplay, Timegram 및 기타 제품과 기능("Incosplay 제품" 또는 "제품")을 제공하기 위해 당사가 처리하는 정보의 내용을 설명합니다. 자세한 도구와 정보는 Incosplay 설정 및 Timegram 설정에서 확인할 수 있습니다.
      </p>

      <section class="pp-section">
        <h2>1. 어떤 유형의 정보를 수집하나요?</h2>
        <p>당사는 Incosplay 제품을 제공하기 위해 귀하에 관한 정보를 처리해야 합니다. 수집하는 정보의 유형은 귀하가 제품을 이용하는 방식에 따라 달라집니다.</p>
        <h3>1.1 귀하와 다른 사람이 제공하는 정보</h3>
        <h4>귀하가 제공하는 정보와 콘텐츠</h4>
        <p>당사는 귀하가 계정을 등록하거나, 콘텐츠를 만들거나 공유하거나, 메시지를 보내거나, 다른 사람과 상호작용하는 등 제품을 이용할 때 제공하는 콘텐츠, 메시지 및 기타 정보를 수집합니다. 여기에는 사진 촬영 위치나 파일 생성일과 같은 메타데이터가 포함될 수 있습니다.</p>
        <h4>커뮤니티와 커뮤니케이션</h4>
        <p>당사는 귀하와 관련된 사람, 해시태그, 계정, 그룹 및 제품 내 상호작용에 관한 정보를 수집합니다. 귀하가 기기에서 주소록, 통화 기록 또는 SMS 등을 다운로드, 동기화 또는 가져오는 경우 연락처 정보를 수집할 수 있습니다.</p>
        <h4>제품 이용 정보</h4>
        <p>당사는 귀하가 보는 콘텐츠, 사용하는 기능, 수행하는 활동, 상호작용하는 사람이나 계정, 활동의 시간, 빈도 및 기간 등 제품 이용 방식에 관한 정보를 수집합니다.</p>
        <h4>제품 내 거래 정보</h4>
        <p>귀하가 제품에서 구매 또는 기타 금융 거래를 하는 경우, 당사는 결제 정보, 계정 및 배송 정보, 연락처 정보 등 구매 또는 거래 정보를 수집합니다.</p>
        <h4>다른 사람이 귀하에 대해 제공하는 정보</h4>
        <p>당사는 다른 사람이 제품을 이용할 때 제공하는 콘텐츠, 메시지 및 정보를 수집하고 분석합니다. 여기에는 다른 사람이 귀하와 사진을 공유하거나, 댓글을 달거나, 메시지를 보내거나, 귀하의 연락처 정보를 업로드, 동기화 또는 가져오는 경우가 포함될 수 있습니다.</p>
        <h3>1.2 기기에서 수집하는 정보</h3>
        <p>당사는 제품과 연동된 컴퓨터, 휴대폰, 연결된 TV 및 기타 인터넷 연결 기기에서 정보와 해당 기기에 관한 정보를 수집하며, 귀하가 사용하는 여러 기기의 데이터를 결합할 수 있습니다.</p>
        <ul>
          <li><strong>기기 속성:</strong> 운영 체제, 하드웨어와 소프트웨어, 배터리 수준, 신호 강도, 메모리, 브라우저 유형, 애플리케이션과 파일 이름 및 유형, 플러그인.</li>
          <li><strong>기기 내 활동:</strong> 창이 전면 또는 백그라운드에 있는지 여부, 마우스 포인터 움직임 등 기기에서의 활동 정보.</li>
          <li><strong>식별자:</strong> 고유 ID, 기기 ID, 계정 ID 및 공유 기기 식별자.</li>
          <li><strong>기기 설정 데이터:</strong> 위치, 카메라 또는 사진 접근 권한 등 귀하가 수신을 허용한 정보.</li>
          <li><strong>네트워크 및 연결:</strong> 통신사 또는 제공업체, 언어, 시간대, 휴대전화 번호, IP 주소, 연결 속도 및 주변 네트워크 정보.</li>
          <li><strong>쿠키 데이터:</strong> 기기에 저장된 쿠키의 데이터, 쿠키 식별자 및 설정.</li>
        </ul>
        <h3>1.3 파트너로부터 받는 정보</h3>
        <p>광고주, 앱 개발자, 게시자 및 기타 파트너는 Incosplay 도구, Incosplay 로그인, API, SDK 또는 픽셀을 사용할 때 당사에 정보를 제공할 수 있습니다. 당사는 파트너가 데이터를 제공하기 전에 이를 수집, 사용 및 이전할 법적 권리를 보유하도록 요구합니다.</p>
      </section>

      <section class="pp-section">
        <h2>2. 이 정보를 어떻게 사용하나요?</h2>
        <p>당사는 귀하의 설정을 기반으로 보유한 정보를 Incosplay 제품 및 관련 서비스를 제공하고 지원하기 위해 사용합니다.</p>
        <h3>2.1 제품 제공, 개인화 및 개선</h3>
        <p>당사는 제품 제공, 기능과 콘텐츠 개인화, 추천 제공, 이용 편의성 향상, 위치 관련 맥락 이해, 제품 개발과 테스트, 광고·제안·스폰서 콘텐츠의 선택 및 개인화를 위해 정보를 사용합니다.</p>
        <h3>2.2 측정, 분석 및 기타 비즈니스 서비스 제공</h3>
        <p>당사는 광고주와 파트너가 광고 및 서비스의 성과와 배포를 측정하고 사람들이 사이트, 앱 및 서비스와 상호작용하는 방식을 이해할 수 있도록 정보를 사용합니다.</p>
        <h3>2.3 보안, 무결성 및 보호 보장</h3>
        <p>당사는 계정과 활동을 확인하고, 유해 행위를 방지하며, 스팸 및 기타 유해 콘텐츠를 식별하고 예방하고, 제품의 무결성과 보안을 개선하기 위해 정보를 사용합니다.</p>
        <h3>2.4 귀하와의 커뮤니케이션</h3>
        <p>당사는 마케팅 제안을 보내고, 제품에 대해 안내하며, 정책과 약관을 알리고, 문의에 응답하기 위해 정보를 사용합니다.</p>
        <h3>2.5 공익을 위한 연구와 혁신</h3>
        <p>당사는 연구 파트너로부터 받은 정보를 포함하여 사회 복지, 기술, 공익, 건강 및 복지와 관련된 연구와 혁신을 수행하고 지원하기 위해 정보를 사용합니다.</p>
      </section>

      <section class="pp-section">
        <h2>3. 이 정보는 어떻게 공유되나요?</h2>
        <p>당사는 다음과 같은 방식으로 귀하의 정보를 다른 사람과 공유합니다.</p>
        <h3>3.1 귀하가 소통하고 공유하는 사람과 계정</h3>
        <p>귀하가 제품을 사용해 정보를 소통하고 공유할 때 공유 대상을 선택합니다. 공개 정보는 계정이 없는 사람을 포함하여 제품 안팎의 모든 사람이 볼 수 있습니다.</p>
        <h3>3.2 다른 사람이 공유하거나 재공유하는 귀하에 관한 콘텐츠</h3>
        <p>제품에서 귀하의 활동을 볼 수 있는 사람은 해당 정보를 다른 사람과 공유할 수 있습니다. 또한 사람들은 제품을 사용해 귀하에 관한 콘텐츠를 만들고 자신이 선택한 대상과 공유할 수 있습니다.</p>
        <h3>3.3 제품 내 활성 상태 또는 존재 정보</h3>
        <p>귀하의 커뮤니티 구성원은 Timegram을 포함한 제품에서 귀하의 활성 상태 또는 마지막 이용 시간을 나타내는 신호를 볼 수 있습니다.</p>
        <h3>3.4 앱, 사이트 및 제3자 연동</h3>
        <p>당사 제품을 사용하거나 제품과 연동된 제3자 앱, 사이트 및 서비스는 귀하가 게시하거나 공유한 정보의 일부를 받을 수 있습니다. 해당 정보의 사용은 해당 서비스의 약관과 정책에 따릅니다.</p>
        <h3>3.5 새로운 소유자</h3>
        <p>당사 제품 또는 그 자산의 전부 또는 일부가 다른 주체의 소유 또는 통제를 받게 되는 경우, 당사는 귀하의 정보를 새로운 소유자에게 이전할 수 있습니다.</p>
        <h3>3.6 제3자 파트너와의 정보 공유</h3>
        <p>당사는 제품 제공과 개선을 돕기 위해 제3자 파트너와 협력합니다. 당사는 귀하의 정보를 판매하지 않으며, 파트너가 당사가 제공하는 데이터를 사용하거나 공개하는 방식을 엄격히 제한합니다.</p>
        <ul>
          <li><strong>분석 파트너:</strong> 게시물, 광고, 페이지, 동영상 및 기타 콘텐츠와의 상호작용에 관한 집계 통계를 받습니다.</li>
          <li><strong>광고주:</strong> 귀하의 허락 없이 개인을 식별할 수 있는 정보를 제공하지 않으며, 광고 대상과 성과에 관한 보고서를 받습니다.</li>
          <li><strong>측정 파트너:</strong> 분석 및 측정 보고서 작성을 위해 집계되는 정보를 받습니다.</li>
          <li><strong>제품 내 상품 및 서비스 제공 파트너:</strong> 구매 완료에 필요한 공개 정보와 거래 정보를 받을 수 있습니다.</li>
          <li><strong>공급업체 및 서비스 제공업체:</strong> 인프라, 분석, 고객 지원, 결제 및 설문조사 등 운영을 지원합니다.</li>
          <li><strong>연구자 및 과학자:</strong> 과학, 혁신, 공익, 건강 및 복지에 기여하는 연구를 위해 정보와 콘텐츠를 받을 수 있습니다.</li>
          <li><strong>법 집행 기관 및 공식 요청:</strong> 아래에 설명된 상황에서 공식 요청에 따라 정보를 받을 수 있습니다.</li>
        </ul>
      </section>

      <section class="pp-section">
        <h2>4. 본인 정보를 어떻게 관리하거나 삭제할 수 있나요?</h2>
        <p>당사는 귀하가 데이터를 열람, 수정, 이전 및 삭제할 수 있도록 합니다. 데이터는 Incosplay 서비스와 제품을 제공하는 데 필요한 기간 또는 계정이 삭제될 때까지 중 먼저 도래하는 시점까지 보관됩니다.</p>
        <p>귀하의 요청에 따라 계정을 삭제하면 귀하가 게시한 정보가 삭제되며 이후 복구할 수 없습니다. 다른 사람이 공유한 귀하에 관한 정보는 귀하의 계정 일부가 아니므로 귀하가 삭제할 수 없습니다.</p>
      </section>

      <section class="pp-section">
        <h2>5. 공식 요청에 대응하거나 피해를 방지하기 위해 어떻게 하나요?</h2>
        <p>당사는 공식 법적 요청에 대응하거나 사기, 무단 사용, 약관 위반, 유해하거나 불법적인 행위 또는 임박한 피해를 방지해야 한다는 선의의 이유가 있는 경우 규제 기관, 법 집행 기관 및 기타 당사자와 정보를 접근, 보존 및 공유할 수 있습니다.</p>
        <p>법적 요청, 법적 의무, 정부 조사, 잠재적 위반 조사 또는 피해 방지 필요성이 있는 경우 당사는 정보를 더 오래 보관할 수 있습니다.</p>
      </section>

      <section class="pp-section">
        <h2>6. 글로벌 서비스 내에서 데이터를 어떻게 처리하고 이전하나요?</h2>
        <p>
          당사는 본 정책에 따라 Incosplay 회사, 외부 파트너 및 귀하가 소통하고 콘텐츠를 공유하는 사람들과 전 세계적으로 정보를 공유합니다. 이러한 이전은
          <a href="http://safari-reader//incosplay.top/agreement" target="_blank" rel="noopener">Incosplay 사용자 계약</a>
          에 명시된 서비스를 제공하고 전 세계에서 제품을 운영 및 제공하기 위해 필요합니다.
        </p>
      </section>

      <section class="pp-section">
        <h2>7. 본 정책의 변경 사항은 어떻게 통지하나요?</h2>
        <p>당사는 본 정책의 변경 사항을 사전에 통지하고, 귀하가 제품을 계속 사용할지 결정하기 전에 개정본을 검토할 기회를 제공합니다.</p>
      </section>

      <section class="pp-section">
        <h2>8. 문의는 어떻게 하나요?</h2>
        <p>본 정책에 대해 궁금한 사항이 있는 경우 아래 방법으로 당사에 문의할 수 있습니다.</p>
        <address class="pp-address">
          연락 이메일:
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
