# Vue 3 + TypeScript + Vite

## eslint 설정과 prettier

> prettier의 `bracketSameLine` 옵션은 JSX의 `>` 기호의 라인을 시작하는 부분과 같은 라인으로 맞출 것인지에 대한 설정을 합니다.  
> eslint 의 `eslint-plugin-vue` 플러그인을 `rules` 필드를 통해 커스텀할 수 있는데 그 중 `vue/html-closing-bracket-newline` 룰이 위에서 언급한 prettier의 `bracketSameLine` 옵션과 불일치를 발생시켜 반복적인 오류해결 루프에 빠질수 있습니다. eslint를 고치면 prettier에러가 나고 prettier에러를 고치면 eslint 에러가 나는 식으로 오류 루프에 빠져버리게 됩니다.  
> 이런 경우 단순하게 처리하는 방법으로 prettier의 `bracketSameLine` 옵션을 사용하지 말거나(default가 false) `false` 로 바꿔 주면 됩니다.
