# Legal Documents

App Store 심사용 법적 문서입니다.

## 파일 구성
- `privacy-policy.ko.html` / `privacy-policy.en.html` — 개인정보처리방침
- `terms.ko.html` / `terms.en.html` — 이용약관(EULA)




2. **공개 URL로 호스팅**
   - 가장 간단한 방법: 이 `legal/` 폴더를 별도 GitHub 퍼블릭 레포지토리에 올리고 GitHub Pages 활성화
   - 또는 기존 `tools/codi-admin` 배포에 `/legal/*.html` 경로로 포함
   - 또는 Notion/Cloudflare Pages에 업로드

3. **App Store Connect 설정**
   - App Information → **Privacy Policy URL** 필드에 `privacy-policy.ko.html` 공개 URL 입력
   - In-App Purchases → 구독 상품 상세 → **EULA** 필드에 `terms.ko.html` URL 입력 (또는 앱 내에서 링크로 제공)

4. **앱 내 링크 연결**
   - 설정 화면 및 Paywall(구독 구매) 화면에 두 문서 링크 배치
   - Paywall에는 **반드시** 다음이 함께 표시되어야 리젝을 피함:
     - 구독명 / 기간 / 가격 / 자동갱신 문구 / 해지 방법
     - "구매 복원(Restore Purchases)" 버튼
     - 개인정보처리방침 링크
     - 이용약관(EULA) 링크

## 문서 내 검토 필요 항목

- [ ] 연락처 이메일 (`{{CONTACT_EMAIL}}`)
- [ ] 시행일자 (현재 2026-04-09로 기재됨 — 실제 배포일로 업데이트)
- [ ] 구독 상품명/가격이 실제 App Store Connect에 등록한 내용과 일치하는지
- [ ] 영문 버전은 해외 마켓 출시할 때만 필요 (한국만 출시하면 KO만으로 충분)
