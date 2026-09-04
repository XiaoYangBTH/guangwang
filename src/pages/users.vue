<script>
export default {
  name: 'HiLiveChildSafetyPolicy',
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
  <div class="csp-wrapper">
    <div class="csp-container" :lang="currentLang">
      <div class="csp-language-switch" aria-label="Language selector">
        <span class="csp-language-label">{{ currentLang === 'en' ? 'Language' : '언어' }}</span>
        <div class="csp-language-options">
          <button
            v-for="option in languageOptions"
            :key="option.value"
            class="csp-language-button"
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
        <header class="csp-header">
          <h1>Nuomet Policy Agreement</h1>
          <p class="csp-updated">
            Last updated: August 19, 2026
          </p>
        </header>

        <p class="csp-intro">
          Nuomet adheres to a zero-tolerance policy for any form of child
          abuse, exploitation, and/or sexual behavior. We are committed to
          protecting the safety of underage users and ensuring that the
          platform is not used for inappropriate behavior. Any users who
          violate the Nuomet Policy will have their accounts
          deleted and may face legal consequences.
        </p>

        <!-- 1. Age Restriction -->
        <section class="csp-section">
          <h2>1. Age Restriction</h2>
          <ul>
            <li>Users must be at least 18 years old to use Nuomet.</li>
            <li>
              Falsifying one's age to access the platform is strictly
              prohibited and will result in the suspension or deletion of the
              account.
            </li>
          </ul>
        </section>

        <!-- 2. Prohibited Activities -->
        <section class="csp-section">
          <h2>2. Prohibited Activities</h2>
          <p>
            Nuomet uses both automated and manual systems to detect underage
            activity and Child Sexual Abuse and Exploitation (CSAE). Any
            attempt to circumvent these systems is strictly prohibited.
            Prohibited activities include, but are not limited to, the
            following:
          </p>

          <h3>Sexualization of Minors and Child Sexual Abuse and Exploitation (CSAE)</h3>
          <ul>
            <li>
              Sharing, creating, or distributing content involving child
              sexual abuse or exploitation.
            </li>
            <li>
              Any content related to minor sexual attraction, such as
              discussions, sexual performances, or wearing sexually suggestive
              clothing.
            </li>
            <li>
              Any form of child nudity or sexually suggestive descriptions,
              including artistic representations such as drawings or
              animations.
            </li>
          </ul>

          <h3>Harmful or Dangerous Behavior Involving Minors</h3>
          <ul>
            <li>
              Threatening, encouraging, or engaging in physical violence
              against minors.
            </li>
            <li>Psychological abuse, coercion, or manipulation of minors.</li>
            <li>
              Depicting or encouraging minors to engage in dangerous
              activities.
            </li>
            <li>Promoting or depicting neglect or trafficking of minors.</li>
          </ul>
        </section>

        <!-- 3. Minor Representation on the Platform -->
        <section class="csp-section">
          <h2>3. Minor Representation on the Platform</h2>
          <ul>
            <li>
              Minors are strictly prohibited from appearing in live streams,
              videos, or any other form of content.
            </li>
            <li>Creating or managing accounts for minors is prohibited.</li>
            <li>Falsifying age to gain access to the platform is prohibited.</li>
          </ul>
        </section>

        <!-- 4. Reporting Mechanism -->
        <section class="csp-section">
          <h2>4. Reporting Mechanism</h2>
          <p>
            Any incidents of child abuse will be reported to the National
            Center for Missing and Exploited Children (NCMEC) or other
            relevant authorities, as required by applicable laws. Users can
            report potential violations via the in-app reporting function or
            by emailing
          </p>
        </section>

        <!-- 5. Prohibited Users -->
        <section class="csp-section">
          <h2>5. Prohibited Users</h2>
          <p>
            Users who have been convicted of child-related crimes (including
            but not limited to sexual assault, physical abuse, neglect, or
            trafficking) are strictly prohibited from using Nuomet.
          </p>
        </section>

        <!-- 6. Enforcement and Transparency -->
        <section class="csp-section">
          <h2>6. Enforcement and Transparency</h2>
          <p>
            Nuomet will strictly enforce the Child Safety Policy, and any
            violations will result in immediate penalties. Depending on the
            severity of the violation, Nuomet may cooperate with law
            enforcement agencies to conduct investigations.
          </p>
        </section>

        <!-- 7. User Education -->
        <section class="csp-section">
          <h2>7. User Education</h2>
          <p>Nuomet educates users about child safety through the following methods:</p>
          <ul>
            <li>Providing the platform's child safety policy.</li>
            <li>
              Offering reminders and alerts during content creation and
              sharing to avoid potential dangers.
            </li>
          </ul>
        </section>

        <!-- 8. Additional Resources -->
        <section class="csp-section">
          <h2>8. Additional Resources</h2>
          <p>
            If you encounter child exploitation or abuse outside of Nuomet, we
            recommend contacting the following resources based on your
            location:
          </p>
          <ul>
            <li>
              <strong>North America, Australia, New Zealand:</strong> National
              Center for Missing and Exploited Children (NCMEC)
            </li>
            <li>
              <strong>Europe:</strong> Law enforcement reporting channels for
              child sexual coercion and extortion
            </li>
            <li>
              <strong>South America and Other Regions:</strong> International
              Centre for Missing &amp; Exploited Children
            </li>
          </ul>
        </section>

        <!-- 9. Commitment to Child Safety -->
        <section class="csp-section">
          <h2>9. Commitment to Child Safety</h2>
          <p>
            Nuomet is committed to continuously evaluating and improving its
            policies, systems, and practices to ensure the highest standards
            of child safety on the platform. Our goal is to provide a safe and
            inclusive space for everyone.
          </p>
        </section>
      </div>
      <div v-else>
        <header class="csp-header">
          <h1>Nuomet 정책 약관</h1>
          <p class="csp-updated">
            최종 업데이트: 2026년 8월 19일
          </p>
        </header>

        <p class="csp-intro">
          Nuomet은 모든 형태의 아동 학대, 착취 및/또는 성적 행위에 대해 무관용 원칙을 적용합니다. 당사는 미성년 사용자의 안전을 보호하고 플랫폼이 부적절한 행위에 사용되지 않도록 최선을 다합니다. Nuomet 정책을 위반한 사용자는 계정이 삭제될 수 있으며 법적 책임을 질 수 있습니다.
        </p>

        <section class="csp-section">
          <h2>1. 연령 제한</h2>
          <ul>
            <li>Nuomet을 이용하려면 사용자는 만 18세 이상이어야 합니다.</li>
            <li>플랫폼에 접근하기 위해 나이를 허위로 표시하는 행위는 엄격히 금지되며, 계정 정지 또는 삭제로 이어질 수 있습니다.</li>
          </ul>
        </section>

        <section class="csp-section">
          <h2>2. 금지 행위</h2>
          <p>Nuomet은 자동화 시스템과 수동 검토 시스템을 모두 사용하여 미성년자 활동 및 아동 성적 학대와 착취(CSAE)를 탐지합니다. 이러한 시스템을 우회하려는 모든 시도는 엄격히 금지됩니다.</p>
          <h3>미성년자의 성적 대상화 및 아동 성적 학대와 착취(CSAE)</h3>
          <ul>
            <li>아동 성적 학대 또는 착취와 관련된 콘텐츠를 공유, 제작 또는 배포하는 행위.</li>
            <li>토론, 성적 행위, 성적으로 암시적인 의복 착용 등 미성년자에 대한 성적 관심과 관련된 모든 콘텐츠.</li>
            <li>그림이나 애니메이션과 같은 예술적 표현을 포함하여 아동 노출 또는 성적으로 암시적인 묘사에 해당하는 모든 콘텐츠.</li>
          </ul>
          <h3>미성년자와 관련된 유해하거나 위험한 행위</h3>
          <ul>
            <li>미성년자에 대한 신체적 폭력을 위협, 조장 또는 실행하는 행위.</li>
            <li>미성년자에 대한 심리적 학대, 강압 또는 조작.</li>
            <li>미성년자가 위험한 활동에 참여하도록 묘사하거나 조장하는 행위.</li>
            <li>미성년자 방임 또는 인신매매를 홍보하거나 묘사하는 행위.</li>
          </ul>
        </section>

        <section class="csp-section">
          <h2>3. 플랫폼 내 미성년자 표시</h2>
          <ul>
            <li>미성년자는 라이브 스트림, 동영상 또는 기타 모든 형태의 콘텐츠에 등장하는 것이 엄격히 금지됩니다.</li>
            <li>미성년자를 위한 계정을 만들거나 관리하는 행위는 금지됩니다.</li>
            <li>플랫폼 접근을 위해 나이를 허위로 표시하는 행위는 금지됩니다.</li>
          </ul>
        </section>

        <section class="csp-section">
          <h2>4. 신고 절차</h2>
          <p>아동 학대 사건은 관련 법률에 따라 미국 실종·착취아동센터(NCMEC) 또는 기타 관련 기관에 신고됩니다. 사용자는 앱 내 신고 기능 또는 이메일을 통해 잠재적 위반 사항을 신고할 수 있습니다.</p>
        </section>

        <section class="csp-section">
          <h2>5. 금지 사용자</h2>
          <p>성폭행, 신체적 학대, 방임 또는 인신매매를 포함하되 이에 국한되지 않는 아동 관련 범죄로 유죄 판결을 받은 사용자는 Nuomet 사용이 엄격히 금지됩니다.</p>
        </section>

        <section class="csp-section">
          <h2>6. 집행 및 투명성</h2>
          <p>Nuomet은 아동 안전 정책을 엄격히 집행하며, 위반 행위는 즉각적인 제재로 이어질 수 있습니다. 위반의 심각성에 따라 Nuomet은 수사 진행을 위해 법 집행 기관과 협력할 수 있습니다.</p>
        </section>

        <section class="csp-section">
          <h2>7. 사용자 교육</h2>
          <p>Nuomet은 다음과 같은 방식으로 사용자에게 아동 안전에 대해 안내합니다.</p>
          <ul>
            <li>플랫폼의 아동 안전 정책 제공.</li>
            <li>콘텐츠 제작 및 공유 과정에서 잠재적 위험을 피할 수 있도록 알림과 경고 제공.</li>
          </ul>
        </section>

        <section class="csp-section">
          <h2>8. 추가 자료</h2>
          <p>Nuomet 외부에서 아동 착취 또는 학대를 발견한 경우, 귀하의 위치에 따라 다음 기관에 연락할 것을 권장합니다.</p>
          <ul>
            <li><strong>북미, 호주, 뉴질랜드:</strong> 미국 실종·착취아동센터(NCMEC)</li>
            <li><strong>유럽:</strong> 아동 성적 강요 및 착취 관련 법 집행 신고 채널</li>
            <li><strong>남미 및 기타 지역:</strong> 국제 실종·착취아동센터</li>
          </ul>
        </section>

        <section class="csp-section">
          <h2>9. 아동 안전에 대한 약속</h2>
          <p>Nuomet은 플랫폼에서 최고 수준의 아동 안전 기준을 보장하기 위해 정책, 시스템 및 운영 방식을 지속적으로 평가하고 개선하는 데 전념합니다. 당사의 목표는 모두에게 안전하고 포용적인 공간을 제공하는 것입니다.</p>
        </section>
      </div>
    </div>

    <!-- 固定悬浮联系信息条 -->
    <div class="csp-floating-bar">
      <span class="csp-floating-label">Contact:</span>
      <a class="csp-floating-email">Nuomet098772@gmail.com</a>
    </div>
  </div>
</template>

<style scoped>
.csp-wrapper {
  position: relative;
  min-height: 100vh;
}

.csp-container {
  max-width: 860px;
  margin: 0 auto;
  padding: 2.5rem 1.5rem 6rem; /* 底部留白，避免被悬浮条遮挡 */
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
    'Helvetica Neue', Arial, sans-serif;
  color: #2b2d33;
  line-height: 1.7;
  font-size: 16px;
}

.csp-language-switch {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 0.75rem;
  margin-bottom: 1.25rem;
}

.csp-language-label {
  color: #6b6f76;
  font-size: 0.9rem;
}

.csp-language-options {
  display: inline-flex;
  padding: 0.2rem;
  border: 1px solid #d7dbe3;
  border-radius: 999px;
  background: #f6f7fa;
}

.csp-language-button {
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

.csp-language-button.is-active {
  background: #d64545;
  color: #fff;
  font-weight: 600;
}

.csp-header {
  border-bottom: 2px solid #e2e4ea;
  padding-bottom: 1rem;
  margin-bottom: 1.5rem;
}

.csp-header h1 {
  font-size: 1.9rem;
  font-weight: 700;
  margin: 0 0 0.4rem;
  color: #1a1c20;
}

.csp-updated {
  font-size: 0.9rem;
  color: #6b6f76;
  margin: 0;
}

.csp-intro {
  background: #f6f7fa;
  border-left: 4px solid #d64545;
  padding: 1rem 1.25rem;
  border-radius: 6px;
  margin-bottom: 2rem;
  font-size: 0.97rem;
}

.csp-section {
  margin-bottom: 2.25rem;
}

.csp-section h2 {
  font-size: 1.3rem;
  font-weight: 700;
  color: #1a1c20;
  border-bottom: 1px solid #e2e4ea;
  padding-bottom: 0.5rem;
  margin-bottom: 1rem;
}

.csp-section h3 {
  font-size: 1.05rem;
  font-weight: 600;
  color: #33363d;
  margin: 1.25rem 0 0.5rem;
}

.csp-section p {
  margin: 0 0 0.9rem;
  text-align: justify;
}

.csp-section ul,
.csp-section ol {
  margin: 0 0 1rem;
  padding-left: 1.5rem;
}

.csp-section li {
  margin-bottom: 0.6rem;
}

.csp-section a {
  color: #d64545;
  text-decoration: none;
  word-break: break-word;
}

.csp-section a:hover {
  text-decoration: underline;
}

/* 固定在页面底部的半透明悬浮条 */
.csp-floating-bar {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
  padding: 0.85rem 1rem;
  background: rgba(0, 0, 0, 0.6);
  backdrop-filter: blur(4px);
  -webkit-backdrop-filter: blur(4px);
  color: #fff;
  font-size: 0.95rem;
}

.csp-floating-label {
  font-weight: 600;
  opacity: 0.85;
}

.csp-floating-email {
  color: #fff;
  text-decoration: underline;
  word-break: break-word;
}

.csp-floating-email:hover {
  opacity: 0.85;
}

@media (max-width: 600px) {

  .csp-language-switch {
    align-items: flex-start;
    flex-direction: column;
    gap: 0.45rem;
  }

  .csp-language-options {
    width: 100%;
  }

  .csp-language-button {
    flex: 1;
    min-width: 0;
  }

  .csp-container {
    padding: 1.5rem 1rem 6.5rem;
    font-size: 15px;
  }

  .csp-floating-bar {
    flex-direction: column;
    gap: 0.15rem;
    padding: 0.7rem 1rem;
    font-size: 0.88rem;
  }
}
</style>
