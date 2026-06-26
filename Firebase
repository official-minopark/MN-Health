import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-app.js";
import { getFirestore, collection, addDoc, getDocs, deleteDoc, doc, query, orderBy } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore.js";
import { getAuth, GoogleAuthProvider, signInWithPopup, signOut, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-auth.js";

const firebaseConfig = {
  apiKey: "AIzaSyBDIgsg99fxj2RFeEeFVD92mNltAweDpd8",
  authDomain: "mn-health.firebaseapp.com",
  projectId: "mn-health",
  storageBucket: "mn-health.firebasestorage.app",
  messagingSenderId: "442489563296",
  appId: "1:442489563296:web:c2a044ee36b1a1c59641c5"
};

const app = initializeApp(firebaseConfig);
export const db = getFirestore(app);
export const auth = getAuth(app);
export const googleProvider = new GoogleAuthProvider();

export { collection, addDoc, getDocs, deleteDoc, doc, query, orderBy, signInWithPopup, signOut, onAuthStateChanged };

// 유저 uid 기반 컬렉션 경로
export function userCol(uid, name) {
  return collection(db, "users", uid, name);
}
export function userDoc(uid, colName, docId) {
  return doc(db, "users", uid, colName, docId);
}
