unordered_map<STATE, int> memo;

int fn(vector<int>& arr) {
    return dp(STATE_FOR_WHOLE_INPUT, arr);
}

int dp(STATE, vector<int>& arr) {
    if (BASE_CASE) {
        return 0;
    }

  if (memo.contains(STATE)) {
        return memo[STATE];
    }

  int ans = RECURRENCE_RELATION(STATE);
    memo[STATE] = ans;
    return ans;
}
