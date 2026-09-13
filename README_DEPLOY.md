# HASHPIXELS Mining Website — Production

Domain target:
https://www.mine.deadpixelslabs.com/

Contract:
0xB35774851217255a5e1ff08a9752101FCC71fFC8

Chain:
Robinhood Chain mainnet (4663)

Important security behavior:
- No automatic wallet connection.
- No `eth_requestAccounts` on page load.
- No seed phrase/private key input.
- No token approval flow.
- Wallet is requested only when the user explicitly presses CONNECT.
- Claim transaction is requested only after a GPU proof is found and the user presses CLAIM & BURN.

Deploy:
1. Extract this folder.
2. Open PowerShell in the folder.
3. `npx.cmd vercel`
4. Create a NEW Vercel project for the mining website (do not use the asset server project).
5. `npx.cmd vercel --prod`
6. Attach `www.mine.deadpixelslabs.com` to the mining project.

Before public launch:
- Activate mining on the HASHPIXELS contract only when ready.
- Test with a wallet that owns a transferable DEAD PIXELS.
- Confirm WebGPU works in current Chrome/Edge over HTTPS.
