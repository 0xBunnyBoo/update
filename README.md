
 export const transactionDemoCode = `
   import { useAccount } from 'wagmi';
   import { TransactionDefault } from '@coinbase/onchainkit/transaction';
   import { Transaction } from '@coinbase/onchainkit/transaction';
   import { WalletDefault } from '@coinbase/onchainkit/wallet';
 
   export default function TransactionDemo() {
 @@ -40,7 +40,7 @@ export const transactionDemoCode = `
     return (
       <>
         {address ? (
           <TransactionDefault contracts={contracts} chainId={84532} />
           <Transaction contracts={contracts} chainId={84532} />
         ) : (
           <WalletDefault />
         )}
